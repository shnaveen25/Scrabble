# scrabble


**Atom snippets which Hold on to something for React.**

 
Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class [Ref](https://reactjs.org/docs/hooks-overview.html).


Basically, A React Component looks :

    import React, { useEffect, useReducer } from 'react';
    import { connect } from 'react-redux';
    import { bindActionCreators } from 'redux';
    
    const initialState = {
      STATE: VALUE
    };
    
    function stateReducer(state, action) {
      switch (action.type) {
        case ACTION_TYPE:
          return {
            ...state,
            STATE: VALUE
          };
        default:
          return state;
      }
    }
    
    const COMPONENT_NAME = (props) => {
      const [state, dispatch] = useReducer(stateReducer, initialState);
      // setState can be achived by dispatching.
      // dispatch({ type: 'ACTION_TYPE', payload: VALUE });
    
      // Similar to componentDidMount and componentDidUpdate:
      useEffect(
        () => {
          // do something after render
    
          // Similar to componentWillUnmount
          return () => {
            // do something when component unmounts
          };
        },
        []
      );
    
      return (
        <div className="container">
    
        </div>
      );
    };
    
    const mapStateToProps = (state) => ({
    
    });
    
    const mapDispatchToProps = dispatch => bindActionCreators({
    
    }, dispatch);
    
    export default connect(
      mapStateToProps,
      mapDispatchToProps
    )(COMPONENT_NAME);

# To make the above step simple

Introducting **Scrabble**.

All you have to do is search and install a package called `Scrabble` on atom.

 - On your Atom editor Simply key-in a pre-defined set of commands . For
   example,    `useHook`
   
 - Select the itom from Plugin.
 - Edit the highlighted section.
 - Tab to move between highlighted sections.
