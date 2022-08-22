### How it works

Trivy Image scanner was used to scan images for vulnerabilities.

#### How does it work
The first step, Trivy was installed.
The next step, The Opened issues on the Repo was first gotten with {{ github.event.issue.body }}
The first and last bracke was removed, then passed into IFS to remove space, It was looped through to give the name of each image, inside the for loop we call the trivy to scan the image, then pass the result to result_output function to save the results as json passing safe and unsafe as the status
