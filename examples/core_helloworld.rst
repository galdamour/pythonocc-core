core_helloworld.py
============

Abstract
---

Howto launch the example ::

  $ python core_helloworld.py

Example output
---

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998677.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998688.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998798.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998871.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998912.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508998970.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1508999014.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1509259659.jpeg

.. image:: images/screenshots/images\screenshots\capture-core_helloworld-1-1509259736.jpeg


Code
---

  from OCC.Display.SimpleGui import init_display
  from OCC.BRepPrimAPI import BRepPrimAPI_MakeBox
  
  display, start_display, add_menu, add_function_to_menu = init_display()
  my_box = BRepPrimAPI_MakeBox(10., 20., 30.).Shape()
  
  display.DisplayShape(my_box, update=True)
  start_display()
