# Eclipse QVTO ModelCopy Technology

#### Installation Instructions
1. Download "Eclipse Modeling Components". Might work with other Eclipse Editions, just make sure you install EMF.
2. Install QVTO 3.6 (currently only on nightly update-site):
   * Help -> Install new Software -> Work with:
     http://download.eclipse.org/mmt/qvto/updates/nightly/3.6.0 (press enter)
   * Select QVTo-NXXXXXXXXXXXX, Next, Next, Accept Licence, Next, Finish.

3. Install ModelCopy Library
    * Like step 2, with the following Update-Site URL:
      http://raw.githubusercontent.com/ingo-budde/ICMT16-ModelCopy/master/de.upb.modelcopy.updatesite/site.xml
    * Select ModelCopy, proceed until Finish.

### Example
1. Import Example Transformation into Workspace
    * Window -> Show View -> Other... -> Plug-in Development -> Plug-ins
    * A new "Plug-ins" view appears (probably at the bottom of the screen).
    * In this view find the item "de.upb.modelcopy.exampletransformation", right-click -> Import As -> Source Project

2. A new project should appear in your Workspace (see Package Explorer View)

3. Open subfolder transforms. You can have a look at the T1.qvto file there.
   * To execute it for the first time, right-click on T1.qvto -> Run As... -> Run Configurations...

4. The "Run Configurations" window opens. On the left-hand side, double-click on "Operational QVT Interpreter".

5. A sub-entry should appear (probably called T1). On the right-hand side select IN and OUT models by clicking on the respective "Browse..." Buttons.
    * Please select "A.ecore" for IN and "B.ecore" for OUT. These files are located in the "model" subfolder of your project.
    * Next press Run in the Bottom-Right corner of the Window.
    * (This now transforms A.ecore into B.ecore using the rules defined in the "T1.qvto" transformation. You can adapt that transformation and inspect B.ecore afterwards.)

