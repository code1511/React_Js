What is Virtual DOM?

React is an open-source JavaScript library for creating UI.The first thing you need to know about what is virtual dom is that “DOM” stands for “Document Object Model”. It represents your application’s UI. As a result,
whenever there is a change in UI, the DOM becomes updated.
Likewise, Virtual DOM is the virtual representation. It surely works faster and more effective and (Real) DOM. What’s more, because DOM only needs few operations, it can reduce the performance cost greatly.
That is to say about What is virtual dom, it’s time for the next essential point:

How does Virtual DOM work in React?

1) Render () function
As Virtual DOM is a node tree listing content, render() function is the very first point of entry. Again, whenever a component changes, it is updated and the render() will turn to a different tree or branch of React elements.
Thanks to this feature, React will know how to update UI in the most effective way!
2)Batch update
This is what React follows to update Virtual DOM. Instead of sending updates for 1 change only, it helps send in a batch. Therefore, performance can run more smoothly and fast


Virtual Dom:

React creates a tree of custom objects representing a part of the DOM. For example, instead of creating an actual DIV element containing a UL element, it creates a React.div object that contains a React.ul object. It can manipulate these objects very quickly without actually touching the real DOM or going through the DOM API. Then, when it renders a component, it uses this virtual DOM to figure out what it needs to do with the real DOM to get the two trees to match.

You can think of the virtual DOM like a blueprint. It contains all the details needed to construct the DOM, but because it doesn't require all the heavyweight parts that go into a real DOM, it can be created and changed much more easily.

Virtual Dom example with real life:


Let's take an example — though a very naive one: If you have something messed up in a room in your home and you need to clean it, what will be your first step? Will you be cleaning your room which is messed up or the whole house? The answer is definitely that you will be cleaning only the room which requires the cleaning. That's what the virtual DOM does.

Ordinary JS traverses or renders the whole DOM instead of rendering only the part which requires changes.

So whenever you have any changes, as in you want to add another <div> to your DOM then the virtual DOM will be created which actually does not do any changes in the actual DOM. Now with this virtual DOM, you will be checking the difference between this and your current DOM. And only the part which is different (in this case the new <div>) will be added instead of re-rendering the whole DOM.

