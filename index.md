
# Signals and slots

## Definition

Signals and slots are used for communication between objects. The signals and slots mechanism is a central feature of Qt and probably the part that differs most from the features provided by other frameworks. Signals and slots are made possible by Qt's

## **Objective**

This exercise follows up to add interactive functionality to the calculator widgets written in the previous homework. The goal is to use Signals and Slots to simulate a basic calculator behavior. The supported operations are *, +, -, /


 -  [**Calculator-Interface**](#calculator-interface)
 
 -  [**Main-Class**](#main-class)
 
 -  [**Dialog1 Result**](#dialog1_result)
 
 -  [**Dialog2**](#dialog2)

-  [**Dialog2 Result**](#dialog2_result)

 -  [**Dialog3**](#dialog3)

-  [**Dialog3 Result**](#dialog3_result)

 -  [**Calculator**](#calculator)

-  [**Calculator_Result**](#calculator_result)
-  
# Calculator-Interface
![Image](Finterface.png)

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


