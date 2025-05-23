---
MTPE: windsonsea
date: 2024-06-11
hide:
  - toc
---

# Create Notebook

Notebook provides an online web interactive programming environment, making it convenient for developers to quickly conduct data science and machine learning experiments.

Upon entering the developer console, developers can create and manage Notebooks in different clusters and namespaces.

1. Click **Notebooks** in the left navigation bar to enter the Notebook list. Click the **Create** button on the right.

    ![click button](../../images/notebook01.png)

1. The system will pre-fill basic configuration data, including the cluster, namespace, queue and priority.

    ![fill forms](../../images/notebook02.png)

1. In the **Resources** page, the system will pre-fill part of configuration data, including the image type, image URL and resource specs, while you can manually add the data and environment settings.

    ![fill forms](../../images/notebook06.png)

1. In the **Advanced** page, you can customize arguments, scheduling policies, analysis, SSH, and auto-saving.
   Adjust these arguments and click **OK**.

    ![fill forms](../../images/notebook07.png)

1. The newly created Notebook will initially be in the **Pending** state, and will change to **Running**
   after a moment, with the latest one appearing at the top of the list by default.

    ![created](../../images/notebook01.png)

1. Click the **┇** on the right side to perform more actions: update arguments, start/stop, clone Notebook, view workload details, and delete.

!!! note

    If you choose pure CPU resources and find that all GPUs on the node are mounted,
    you can try adding the following container environment variable to resolve this issue:

    ```config
    NVIDIA_VISIBLE_DEVICES=""
    ```
