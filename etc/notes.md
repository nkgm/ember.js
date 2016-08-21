# ember-metal/lib/platform.js

- exports:
    - create (Object.create)
    - defineProperty (not directly set on Object - just exported)
    - hasPropertyAccessors (=hasES5CompliantDefineProperty)
    - canDefineNonEnumerableProperties (=hasES5CompliantDefineProperty)
    - platform (pojo with defineProperty and hasPropertyAccessors)

# ember-views/lib/views/core_view.js

- extends:
    - EmberObject
    - Evented
    - ActionHandler
  
- members
    - **abstract:**
        - clearRenderedChildren
        - _transitionTo
        - destroyElement
    
    - init
    - parentView
    - _state
    - _parentView
    - concreteView
    - instrumentName
    - instrumentDetails
    - trigger
    - has
    - destroy
    
    - **reopenClass:**
        - renderer
        
# packages/ember-runtime/lib/system/core_object.js
