# City-level Transmission (CLT) Base Model

> ***The CLT base model is a mathematical framework and modular codebase for scalable compartmental models of respiratory virus transmission in a city. This model is written by the [Meyers Lab](http://www.bio.utexas.edu/research/meyers/) and [epiENGAGE center](https://www.cdc.gov/insight-net/php/implementers/index.html).***

The mathematical framework is inspired by the immunoSEIRS model of the Meyers Lab (see [Bi and Bandekar et al. 2023](https://www.researchgate.net/publication/375193467_Scenario_Projections_for_SARS-CoV-2_Influenza_and_RSV_Burden_in_the_US_2023-2024), [Bi et al. 2022](https://repositories.lib.utexas.edu/server/api/core/bitstreams/da7bb152-3343-4135-86e3-040546d6e5b5/content) and [Bouchnita et al. 2021](https://repositories.lib.utexas.edu/items/e8d50517-6e78-488b-8c95-8c1138d90c28) for some related recent publications).

Documentation is created by Linda Pei ("LP"). Base model code is created by LP in collaboration with Shuotao "Sonny" Diao, Remy Pasco, and Emily Javan, and with supervision from Dave Morton and Lauren Meyers. Special thanks to Cary Murray for generous guidance on software engineering design. 

## Codebase layout

    README.md               # Read me! :) 

    base_components.py      # Base classes used to create a compartmental model.

    flu_components.py       # A specific S-E-I-H-R-D model for influenza.

    flu_tests.py            # Suite of pytest tests for flu_components.py

    flu_demo.py             # Demo implementation of flu_components.py
                              flu model for tutorial and testing purposes.  

    flu_demo_input_files    # Collection of .json and .csv files used as 
                              input values for flu_demo.py. These values are
                              "toy" predefined values for demo purposes only. 
                              Realistic applications will use estimation 
                              and calibration from real-world data. 

