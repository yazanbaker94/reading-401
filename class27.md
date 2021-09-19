When you have multiple contexts, what component type should you use (class/function) and why?
function, because you can use a Context.Consumer

What are some good use cases for using the Context API for global state?

But first of all, what is a global state anyway? As we know, the typical way to pass data between disconnected components is through prop drilling. This is fine for a couple of levels down the component tree. But as soon as the complexity grows, so does the need for a global state. Imagine a component needing data that lies five levels above in the component tree. Passing props into each component on the way down would quickly become a nightmare. In addition to writing a lot of unnecessary code we would also give each component properties they will never use, which undoubtedly would become a huge mess. A global state would solve this by keeping a state at the top level and provide access methods to all child levels without the need to pass props.


How can you best test context?


                    import React from 'react'
                    import {render, screen} from '@testing-library/react'
                    import '@testing-library/jest-dom'
                    import {NameContext, NameProvider, NameConsumer} from '../react-context'

                    /**
                     * Test default values by rendering a context consumer without a
                     * matching provider
                     */
                    test('NameConsumer shows default value', () => {
                      render(<NameConsumer />)
                      expect(screen.getByText(/^My Name Is:/)).toHaveTextContent(
                        'My Name Is: Unknown',
                      )
                    })

                    /**
                     * A custom render to setup providers. Extends regular
                     * render options with `providerProps` to allow injecting
                     * different scenarios to test with.
                     *
                     * @see https://testing-library.com/docs/react-testing-library/setup#custom-render
                     */
                    const customRender = (ui, {providerProps, ...renderOptions}) => {
                      return render(
                        <NameContext.Provider {...providerProps}>{ui}</NameContext.Provider>,
                        renderOptions,
                      )
                    }

                    test('NameConsumer shows value from provider', () => {
                      const providerProps = {
                        value: 'C3PO',
                      }
                      customRender(<NameConsumer />, {providerProps})
                      expect(screen.getByText(/^My Name Is:/)).toHaveTextContent('My Name Is: C3P0')
                    })

                    /**
                     * To test a component that provides a context value, render a matching
                     * consumer as the child
                     */
                    test('NameProvider composes full name from first, last', () => {
                      const providerProps = {
                        first: 'Boba',
                        last: 'Fett',
                      }
                      customRender(
                        <NameContext.Consumer>
                          {value => <span>Received: {value}</span>}
                        </NameContext.Consumer>,
                        {providerProps},
                      )
                      expect(screen.getByText(/^Received:/).textContent).toBe('Received: Boba Fett')
                    })

                    /**
                     * A tree containing both a providers and consumer can be rendered normally
                     */
                    test('NameProvider/Consumer shows name of character', () => {
                      const wrapper = ({children}) => (
                        <NameProvider first="Leia" last="Organa">
                          {children}
                        </NameProvider>
                      )

                      render(<NameConsumer />, {wrapper})
                      expect(screen.getByText(/^My Name Is:/).textContent).toBe(
                        'My Name Is: Leia Organa',
                      )
                    })
                    
                    
                    
Document the following Vocabulary Terms
Term
context

React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.



useContext()

“useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props

static context


The contextType property is used to consume a context created with React. ... When the property is specified for a React component, you can access the current value of the context using this. context inside lifecycle methods of the component.

