<!--
{% comment %}
Copyright 2018-2021 Elyra Authors

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
{% endcomment %}
-->

# Elyra Component Library - The Component Library for AI, Machine Learning, ETL, and Data Science

   This is a component library for artificial intelligence, machine learning,
   "extract, transform, load" processes and data science.
   The goal is to enable low-code/no-code rapid prototyping by providing
   ready-made components for various business domains,
   supporting various computer languages, working on various data flow editors and
   running on diverse execution engines.
   To demonstrate its utility, we constructed a workflow composed exclusively of this library's components.
  To demonstrate the capabilities of this library, we made use of a publicly available Computed Tomography (CT) scans dataset
   and created a deep learning model, which is supposed to classify exams as either
   COVID-19 positive or negative. The pipeline was built with Elyra's Pipeline Visual Editor,
   with support for local, Airflow and Kubeflow execution [https://arxiv.org/abs/2103.03281](https://arxiv.org/abs/2103.03281).


Components of this library can be exported as:
1. KubeFlow pipeline components
2. Apache Airflow components
3. Standalone graphical components for the Elyra pipeline editor
4. Standalone components to be run from the command line

![Visually create pipelines from notebooks and run everywhere](https://github.com/IBM/claimed/raw/master/images/elyra_graphical_export.png)
*Visually create pipelines from notebooks and run everywhere*

Each notebook is following a similar format.

1. The first cell contains a description of the component itself.
2. The second cell installs all dependencies using pip3.
3. The third cell imports all dependencies.
4. The fourth cell contains a list of dependencies, input parameters, and return values as Python comments
5. The fifth cell reads the input parameters from environment variables.


![Export notebooks and files as runtime components for different engines](https://github.com/IBM/claimed/raw/master/images/elyra_cli_export.png)
*Export notebooks and files as runtime components for different engines*


To learn more on how this library works in practice, please have a look at the following [video](https://www.youtube.com/watch?v=FuV2oG55C5s)

.. [covidata] Joseph Paul Cohen et al. *COVID-19 Image Data Collection: Prospective Predictions Are the Future*, arXiv:2006.11988, 2020

