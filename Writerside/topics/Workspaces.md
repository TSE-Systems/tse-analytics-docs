# Workspaces

A *Workspace* in TSE Analytics is a project file that contains all data, analysis settings, results, and visualizations related to your experiment.

A *Workspace* comprises all datasets (one or multiple) listed in the Dataset tab including copies of imported datasets and merged datasets as well automatically extracted meta-data and settings which have been edited after import.
These include animal information, factors, plot settings, settings for time binning (including light/dark phases and custom time phases), animal selection, exclusion of animals and exclusion of time phases. 


**Save Workspace**

The report for each dataset is saved within a workspace and is restored when opening the workspace. 
A *Workspace* can be saved via **File | Save Workspace** or by clicking the **Save Workspace** button. 

![Figure: Saving Workspace.png](Saving Workspace.png)

> **Important**: A workspace must be saved manually as described above before closing the software since workspaces are not saved automatically.
> All changes made to a workspace will be lost if the workspace has not been saved before closing or exiting the software. 
{style = 'warning'}


**Open Workspace**

![Figure: Open Workspace.png](Open Workspace.png)

To open an existing workspace, you can:

- Select **File → Open Workspace** from the main menu, or

- Click the **Open Workspace** button on the toolbar.

If you have used a workspace recently, you can quickly reopen it by selecting **File → Open Recent**. This option displays a list of your most recently accessed workspaces for easy access.

> **Important**: Graphs, statistical analysis results, split modes, variable selection and outlier detection settings are NOT saved within a workspace and will be deleted or reset when closing TSE Analytics even if a workspace has been saved.
{style = 'warning'}

Please ensure to either export graphs and analysis result manually or to add the respective graphs and tables to the report followed by either saving/ printing the report or saving the workspace.

> **Note**: The software layout (selection and arrangement of widgets) is not workspace specific.
> The layout of the last session will be restored when opening TSE Analytics again, independent of the loaded datasets or workspaces.
{style = 'note'}
