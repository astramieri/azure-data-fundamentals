# Explore Microsoft Fabric

**Microsoft Fabric** is a unified software-as-a-service (SaaS) offering with all your data stored in a single open format in OneLake.

**OneLake** is Fabric's lake-centric architecture that provides a single, integrated environment for data professionals and the business to collaborate on data projects. Think of it like **OneDrive for data**.

OneLake combines storage locations across different regions and clouds into a single logical lake, without moving or duplicating data. Data can be stored in any file format in OneLake and can be structured or unstructured. For tabular data, the analytical engines in Fabric will write data in delta format when writing to OneLake. All engines will know how to read this format and treat delta files as tables no matter which engine writes it.