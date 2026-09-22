# Mission Reflection

Object storage is better suited for storing millions of photos because it is designed to handle large amounts of unstructured data such as images, videos, and backups. Unlike a traditional block storage hard drive, object storage organizes data as objects inside buckets and is suitable for applications that need to store many files. It can also make the data easier to access and manage as the amount of stored data grows.

Using Docker made it easier to deploy the MinIO storage server because I did not have to install and configure all the required components manually. With one Docker command, I was able to download the MinIO image, create the container, set the administrator credentials, and expose the ports needed to access the Web Console. This made the deployment process faster and more organized.

A bucket is a storage container used to organize and store objects in cloud object storage. In this activity, I created a bucket named `client-photos` and uploaded `nature.jpg` inside it. The bucket provided a specific place where the sample file could be stored and managed.

Large enterprise companies can help prevent data loss by keeping copies of their object storage data in different locations or on multiple physical systems. They can also use backups and replication so that if one physical server crashes, another copy of the data can still be available. These practices help reduce the risk of permanently losing important files.

My confidence in navigating the Linux command line is growing because I have become more familiar with running Docker commands, checking containers, and working with cloud services. At first, the commands were unfamiliar, but completing the activities step by step helped me understand what each command does. I am now more comfortable using the terminal and feel that I can continue learning more Linux commands.