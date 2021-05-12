# CMR physics challenge

| [Home](index.md) | [Physics challenge](CMR-physics-challenge.md) | [DL recon challenge](CMR-deep-learning-reconstruction-challenge.md) | [Material](encrypted.html) | [Tutorial I](Tutorial_session.md) | [Tutorial II/Awards](Awards_Session.md) |

## Description
Pulse sequences in MRI describe all components that are necessary to acquire an MR image with the desired contrast. The beauty of MRI is that by virtue of using different pulse sequences, different imaging information can be obtained, allowing for comprehensive assessment of the tissue in question. However, at the same time, inadvertently chosen pulse sequences lead to artifacts and can make the images unusable. In particular in cardiac MR, the righ pulse sequence choice is crucial for adequate image quality due to a number of artifact sources including motion and flow artifacts.

## Challenge
In this challenge you get to work with a spoiled gradient echo sequence (spGRE). The coding challenge is based on a script that simulates the effect of the pulse sequence on the MR image. Your task is to amend the basic spGRE sequence in such a way that it becomes resilient to flow artifacts. The script simulates the sequence based on gradient traces on three axes and a single trace for the RF pulse. What components can be added and how can those traces be modified to create flow compensated imaging? How do the simulated image results change in response to your sequence developments? Help our virtual radiographers and save the day by eliminating artifacts with the power of pulse sequence development!

## Code
[https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge](https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge)

## Submission
Deadline: Wednesday 19th of May 2021, 23:59 UTC

Please fill out the [submission form](https://docs.google.com/forms/d/e/1FAIpQLSf8k7CmFahOMK5AIYrwbP6-JGJQtZlaQukiGHiI18ZwEKLiLw/viewform?usp=sf_link):
- **Abtract:** Provide a short abstract (max. 150 words) about your solution
- **Figure:** Upload an overview figure depicting your final pulse sequence as well as the simulated imaging result
- **Results:** Upload your results as `*.npz` file containing the modified pulse sequence code.

## Solution
The solution will be discussed and presented in the live session on Thursday, May 20 2021 at 18:00 - 19:00 UTC, and the challenge winners will be announced.
