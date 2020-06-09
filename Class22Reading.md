# class-readings-22-github.io

Describe a case where snapshot testing would be useful, and describe another case where it would be ineffective.

Snapshot testing  will be useful when we have fully working UI and we are refactoring.Whereas 
its not useful if we are making a lot of changes
and the snapshot will not be of any use.

What is the difference between full mount and shallow mount?

Full mounting allows you render the entire component as well as any children components. 
This allows you to fully test the current component and any components it imports.
Shallow mounting minimized the render of any imported components, 
and instead focuses on fully rendering the current component only.

What does npm run build do?

It builds the application
