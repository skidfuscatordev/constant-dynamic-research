Java String Encryption Performance Enhancement with JDK11+
==========================================================

With the help of @xxdark we did a funny. 

Welcome to our GitHub repository where we explore the untapped potential of JDK11+'s `ConstantDynamic` feature to supercharge the performance of string encryption in Java applications. Whether you're a fellow coder curious about Java internals or a seasoned developer looking for ways to secure your Java apps more effectively, you're in the right place.

![Click here to see the draft paper](https://github.com/skidfuscatordev/constant-dynamic-research/blob/main/ConstantDynamicPaper%20v3.pdf)

Overview
--------

This project investigates an innovative approach to string encryption, aimed at reducing the performance overhead typically associated with obfuscation techniques while maintaining high security standards. Using the `ConstantDynamic` feature introduced in JDK11, we've developed a method that cleverly enhances the efficiency and invisibility of string encryption, crucial for protecting sensitive information in Java applications.

Why ConstantDynamic?
--------------------

Before JDK11, obfuscating constant data like strings in Java applications often led to performance penalties due to the computational cost of decryption routines. However, with `ConstantDynamic`, we can now store results of computed constants directly in the JVM's constant pool, allowing these values to be computed only once and reused without reevaluation.

Key Features
------------

*   **Performance Efficiency:** Drastically reduces the overhead from traditional string encryption methods.
*   **Invisibility:** Does not alter class mappings or method signatures.
*   **Context-Sensitive Encryption:** Leverages control flow context to enhance security further.

Performance Insights
--------------------

Our empirical evaluations show a significant performance improvement, with minimal degradation compared to non-obfuscated counterparts. 

![chart (1)](https://github.com/skidfuscatordev/constant-dynamic-research/assets/30368557/9e820c3d-762f-49bc-b038-ecd158a758b9)

Acknowledgments
---------------

A shoutout to the vibrant Recaf community and all contributors to the field, especially those who have explored the depths of JDK's undocumented behaviors to bring this innovation to light.

License
-------

This project is distributed under the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.
