# resource-view-customization-uwp

Resource view customization for a native Universal Windows Platform (UWP) sample application.

Overview
--------
This repository demonstrates how to customize the resource view in a UWP app that uses a simple scheduler sample. The intent is to show practical techniques for adapting built-in scheduler resource views, styling resource tiles, and extending templates to display custom metadata and visuals for resources.

Key features
------------
- Native UWP sample project (C#) with a Scheduler view and simple view-model bindings.
- Example `Behavior` demonstrating how to attach customization logic without heavy code-behind changes.
- Clear folder layout and minimal dependencies so you can copy and adapt the resource-view customization into your own projects.

Repository structure
--------------------
- `ScheduleUWP/` — Visual Studio solution and project for the sample app.
	- `App.xaml`, `MainPage.xaml` — application and entry UI.
	- `Behavior/SchedulerBehavior.cs` — sample behavior that modifies the scheduler/resource presentation.
	- `ViewModel/SchedulerViewModel.cs` — basic data and binding objects used by the sample.
	- `Assets/`, `Properties/` — project assets and metadata.

Building and running
--------------------
1. Open `ScheduleUWP\ScheduleUWP.sln` in Visual Studio 2019/2022.
2. Restore any NuGet packages if prompted.
3. Set the `ScheduleUWP` project as the startup project and deploy to Local Machine (x86/x64/ARM as appropriate).

How to use this sample
----------------------
- Inspect `SchedulerBehavior.cs` to see how the resource templates are discovered and replaced at runtime.
- Modify `MainPage.xaml` resource templates to change layout or add visual indicators (colors, icons, counts).

Contributing
------------
Contributions and improvements are welcome. If you open issues or pull requests, please include a short description and screenshots where helpful.

License
-------
This sample is provided for demonstration and learning purposes. Check the project properties for any licensing notes before using it in production.

Contact
-------
If you have questions or need help adapting this sample, open an issue in the repository and provide environment details and a short description of what you are trying to achieve.