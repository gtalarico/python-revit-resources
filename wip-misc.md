# Python For Revit

##### A collection of resources for Python-Revit lovers

# Summary

* [Resources](resources.md)
* [Common Questions](common-questions.md)


# Frequently Asked Questions

---

##### What are the out-of-the-box lines in the Dynamo?

```py
import clr  
# imports Common Language Runtime library .This will serve as a bridge between python and the .NET wold
# See this: http://ironpython.net/documentation/dotnet/dotnet.html

clr.AddReference('ProtoGeometry')
# Loads the Protogeometry dll (.net assembly) so Python can use it

from Autodesk.DesignScript.Geometry import *
# Imports Geometry Classes from the DesignScript assembly (Protogeometry)
# this gives you access to Dynamos built in Geometry classes and more.

dataEnteringNode = IN
# This is just telling data entering this node will be stored in a variable called IN.
# You don't actually need this. Go ahead and delete it, nothing will change.
```

##### Recommended reading

* Iron Python Documentation
  * http://ironpython.net/documentation/dotnet/dotnet.html
* DesignSCript Syntax
  * http://dynamoprimer.com/en/07\_Code-Block/7-2\_Design-Script-syntax.html
* DesignScript Guide
  * [http://dynamobim.org/wp-content/uploads/.../Dynamo\_language\_guide\_version\_1.pdf](http://dynamobim.org/wp-content/uploads/forum-assets/colin-mccroneautodesk-com/07/10/Dynamo_language_guide_version_1.pdf)
  *

---

##### Where can I find the list of modules in the Revit API?

You can download the Full API Documentation as well as many examples \(no python examples, unfortunatelly\) from the Autodesk [Developer Network's website](http://usa.autodesk.com/adsk/servlet/index?siteID=123112&id=2484975)

The official documentation is also avaiable online at: [RevitAPIdocs.com](/RevitAPIdocs.com)
