##  View Hooks


 * willInsertElement
 * didInsertElement
 * willDestroyElement
 * willClearRender
 * becameVisible
 * becameHidden

Note:

 * willInsertElement:
 This hook is called after the view has been rendered but before it has been inserted into the DOM. It does not provide access to the view's element.

 * didInsertElement:
 This hook is called immediately after the view has been inserted into the DOM. It provides access to the view's element and is most useful for integration with an external library. Any explicit DOM setup code should be limited to this hook.

 * willDestroyElement:
 This hook is called immediately before the element is removed from the DOM. This is your opportunity to tear down any external state associated with the DOM node. Like didInsertElement, it is most useful for integration with external libraries.

 * willClearRender:
 This hook is called immediately before a view is re-rendered. This is useful if you want to perform some teardown immediately before a view is re-rendered.

 * becameVisible:
 This hook is called after a view's isVisible property, or one of its ancestor's isVisible property, changes to true and the associated element becomes visible. Note that this hook is only reliable if all visibility is routed through the isVisible property.

 * becameHidden:
 This hook is called after a view's isVisible property, or one of its ancestor'sisVisible property, changes to false and the associated element becomes hidden. Note that this hook is only reliable if all visibility is routed through the isVisible property.
