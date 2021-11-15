
# Signals and slots

## Definition

Signals and slots are used for communication between objects. The signals and slots mechanism is a central feature of Qt and probably the part that differs most from the features provided by other frameworks. Signals and slots are made possible by Qt's

## **Objective**

This exercise follows up to add interactive functionality to the calculator widgets written in the previous homework. The goal is to use Signals and Slots to simulate a basic calculator behavior. The supported operations are *, +, -, /


 -  [**Calculator-Interface**](#calculator-interface)
 
 -  [**Main-Class**](#main-class)
 
 -  [**Calculator**](#calculator)
 
 -  [****](#)

-  [****](#)

 -  [****](#)

-  [****](#)

 -  [****](#)

-  [****](#)
-  
# Calculator-Interface
![Image](Finterface.png)

For now our `application` has no reactivity. The goal of the rest of the section is to obtain step/step a fully functional widget.

# Main-Class

```c++
int main(int argc, char *argv[])
{
    QApplication a(argc, argv);
    Calculator w;
    w.setWindowTitle("Calculator");
    w.resize(250,250);
    w.show();
    return a.exec();
}
```
# Calculator
In order to have a computing functionality, we will represent any mathematical operation by:
```
                                               left   (operation)  right
                                           ex:  3          +         9
```


