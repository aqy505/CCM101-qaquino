# Mission Reflection

During this laboratory activity, I learned that checking the server's resources is important even when the containers are running properly. The server still needs enough RAM and disk space to handle user requests and store files and logs. If the resources become full, the application may slow down or stop working, especially when many users access it at the same time.

I also learned how the `docker logs` command can help when a user reports a problem logging into a web application. By checking the logs, I can see the requests made to the application and look for errors that may explain the problem. For example, in this activity, I found an error when I tried to access a page that did not exist. This helped me understand how logs can give useful details when fixing problems.

Logs and metrics are both important, but they show different information. Logs show the events and errors that happen inside an application, while metrics show numbers such as CPU usage and memory consumption. Using both helps me understand what is happening in the system and check if the container is working properly.

For companies that manage thousands of containers, tools like Prometheus and Grafana can help collect and display monitoring data in one place. This makes it easier for engineers to check the condition of many containers without checking each one manually. They can also notice possible problems and respond more quickly.

Overall, this activity helped me improve my troubleshooting skills in a Linux environment. I became more familiar with commands for checking system resources, viewing Docker logs, and monitoring container performance. At first, some commands were new to me, but following the steps helped me understand their purpose. I learned that troubleshooting should be based on actual information from logs and metrics instead of guessing what caused the problem.
