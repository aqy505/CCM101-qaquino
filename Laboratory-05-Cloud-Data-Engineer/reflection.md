# Mission Reflection

Object Storage is better suited for storing millions of photos because it is designed to handle large amounts of unstructured data such as images, videos, and backups. Unlike traditional Block Storage, objects are stored with their data, metadata, and unique identifiers. This makes it easier to organize and manage a large number of files. It can also scale as the amount of stored data continues to increase.

Using Docker made deploying the MinIO storage server easier because I did not need to manually install and configure the entire application. With a Docker command, I was able to start the MinIO server, configure its login credentials, and map the required ports. This showed me how containers can make the deployment process faster and more consistent.

A bucket in cloud storage is a container used to organize and store objects such as images, documents, and other files. During this activity, I created the `client-photos` bucket and uploaded a sample file into it. It helped me understand how cloud storage services organize data instead of using normal folders like a traditional file system.

Large companies need to make sure that their data is still available even if a physical server fails. I think they can achieve this by keeping multiple copies of their data across different servers or locations and by using backups. This reduces the risk of losing important files when hardware problems happen.

My confidence in using the Linux command line is growing as I complete more cloud computing activities. I am becoming more familiar with running Docker commands, checking containers, and understanding terminal outputs. At first, some commands were confusing, but practicing them in KillerCoda has helped me understand what they do. My experience from this mission also makes me more comfortable working with Linux and cloud technologies.