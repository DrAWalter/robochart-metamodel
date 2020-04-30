# robochart-metamodel [![wercker status](https://app.wercker.com/status/d4e803180bb76499fd095643b434bfa4/s/master "wercker status")](https://app.wercker.com/project/byKey/d4e803180bb76499fd095643b434bfa4)
This repository contains the eclipse plugins that implement that metamodel of RoboChart.

The metamodel can be found in circus.robocalc.robochart.parent/circus.robocalc.robochart/model/robochart.ecore

### Development platform requirements ###

* Eclipse 2019-06
* Xtext 2.18.0 can be found in the standard repository in http://download.eclipse.org/modeling/tmf/xtext/updates/composite/releases/ but the option "Show only the latest versions of available software" needs to be unchecked. 
* Maven
* Git

### Build (maven) ###

        1. mvn clean install

### Build (eclipse) ###

        1. Right click circus.robocalc.textual.robochart/model/RoboChart.genmodel 
            1. click 'reload'
            2. select 'Ecore model' and click 'Next'
            3. click 'Next'
            4. click 'Finish'
        2. In the open RoboChart.genmodel      
            1. right click the item 'RoboChart' and select 'Generate Model Code'
            2. right click the item 'RoboChart' and select 'Generate Edit Code'
            3. right click the item 'RoboChart' and select 'Generate Editor Code'

### Run (eclipse) ###

        1. Right click circus.robocalc.robochart.parent
            1. select 'Run As'
            2. double click 'Eclipse Application'
        2. Select the new configuration
            1. click 'Run'
            
### Protocol for updating the tool ###

Whenever updating the tool, follow these steps:

        1. Run Maven with Tests
        2. Change the language reference manual
        3. Change the tool manual

If changes to documentations are not possible immediately, create issues indicating exactly what needs to be done.