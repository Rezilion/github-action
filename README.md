![RezilionLogo](https://user-images.githubusercontent.com/94110576/202431540-dfc99e77-69f4-4360-97db-b6bdc924455a.png)


With Rezilion orb, applications can be built securely by validating vulnerabilities early in the development process. 

developers can focus on exploitable vulnerabilities and reduce their backlog and patching by 85%. 

With Rezilion, you’ll gain a deep understanding of your environment, uncover and validate vulnerabilities in your applications and container images, 
explore dependencies and licenses, and export the output in auditing formats. 

To use this action, you need a Rezilion license.

## Installation guide
1. Install the Rezilion Extension from the following link: https://github.com/marketplace/actions/rezilion
2. Add a Rezilion environment variable:
"REZILION_LICENSE_KEY"
3. Edit your pipeline yml:

      a. Add Rezilion license key variable per required Job
      ```
      name: test
    on: [push]
    jobs:
      test_sanity:
        runs-on: ubuntu-latest
        container:
          image: nginx:latest
    ```

     b. Add Rezilion as a step for each command in your pipeline

     ![image](https://user-images.githubusercontent.com/94110576/210215925-e33e1193-fc82-4bc4-be34-32bc90858b3e.png)

4. Add Rezilion as a Job

    ![image](https://user-images.githubusercontent.com/94110576/210216072-aba96482-6943-4d96-be49-454b51b41d43.png)


    * Make sure to add inside the "needs" field all the Jobs Rezilion Validate is used in

For full user guide, please follow this link:
