# Reflection

In this laboratory activity, I learned how automation can make cloud operations easier and more efficient. When managing hundreds of cloud servers, doing tasks manually can take a lot of time and may lead to mistakes. Using Bash scripts and Cron allows repeated tasks, such as creating backups, to run automatically without needing someone to execute them every time.

However, automation also has risks. A small mistake in a script can affect many systems, especially when the script runs across hundreds or thousands of servers. For example, a destructive command or incorrect file path could cause important data to be deleted. This is why scripts should be checked and tested carefully before scheduling or deploying them on multiple systems.

Writing a Bash script was different from creating a Docker Compose YAML file in Mission 6. In this activity, I used Bash commands to perform steps such as creating directories, assigning variables, and compressing files into a backup archive. Docker Compose, on the other hand, uses YAML to define and manage application services and their configurations. Both tools help automate tasks, but they serve different purposes.

Looking back at my GitHub portfolio from Laboratory 1 to Laboratory 9, I can see how my understanding of cloud computing has developed. At first, I was still learning the basic concepts and tools. As I completed more activities, I gained experience with cloud infrastructure, containers, application deployment, monitoring, security, and automation. These activities helped me understand how different parts of cloud computing work together.

Among the roles I explored, I enjoyed the Cloud Automation Engineer role because I could create a script that performs tasks automatically. It was satisfying to see the backup file created and the Cron schedule configured. Overall, this mission taught me that automation is useful, but it must be handled carefully to keep systems and data safe.