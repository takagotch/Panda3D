### panda3d
---
https://github.com/panda3d/panda3d

https://www.panda3d.org/

```py
// tests/ode/test_ode_joints.py

def test_odejoint_attach_both(world):
  from panda3d import ode
  
  body1 = ode.OdeBody(world)
  body2 = ode.OdeBody(world)
  
  assert len(body1.joints) == 0
  assert len(body2.joints) == 0
  
  joint = ode.OdeBallJoint(world)
  joint.attach(body1, body2)
  
  assert tuple(body1.joints) == (joint,)
  assert tuple(body2.joints) == (joint,)

```

```
```

```
```

