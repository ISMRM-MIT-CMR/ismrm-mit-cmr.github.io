# CMR physics tutorial and challenge

<nav>
  <ul>
    <table>
    <tr>
    {% for nav in site.data.nav %}
      {% if nav.subcategories != null %}
        <td>
          <a href="{{ site.url }}{{ nav.href }}">{{ nav.title }} ▼</a>
          <ul>
          {% for subcategory in nav.subcategories %}
            <li><a href="{{ site.url }}{{ subcategory.subhref }}">{{ subcategory.subtitle }}</a></li>
          {% endfor %}
          </ul>
        </td>
      {% elsif nav.title == page.title %}
         <td class="active">
           <a href="{{ nav.url }}">{{ nav.title }}</a>
         </td>
      {% else %} 
        <td>
          <a href="{{ site.url }}{{ nav.href }}">{{ nav.title }}</a>
        </td>
      {% endif %}
    {% endfor %}
      </tr>
    </table>
  </ul>
</nav> 

## Tutorial
Pulse sequences in MRI describe all components that are necessary to acquire an MR image with the desired contrast. The beauty of MRI is that by virtue of using different pulse sequences, different imaging information can be obtained, allowing for comprehensive assessment of the tissue in question. However, at the same time, inadvertently chosen pulse sequences lead to artifacts and can make the images unusable. In particular in cardiac MR, the righ pulse sequence choice is crucial for adequate image quality due to a number of artifact sources including motion and flow artifacts.

### Code Tutorial
[https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge](https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge)

CMR Physics: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ISMRM-MIT-CMR/CMR-physics-challenge/blob/master/ISMRM_final_live.ipynb)

## Challenge
In this challenge you get to work with a spoiled gradient echo sequence (spGRE). The coding challenge is based on a script that simulates the effect of the pulse sequence on the MR image. Your task is to amend the basic spGRE sequence in such a way that it becomes resilient to flow artifacts. The script simulates the sequence based on gradient traces on three axes and a single trace for the RF pulse. What components can be added and how can those traces be modified to create flow compensated imaging? How do the simulated image results change in response to your sequence developments? Help our virtual radiographers and save the day by eliminating artifacts with the power of pulse sequence development!

### Code Challenge
[https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge](https://github.com/ISMRM-MIT-CMR/CMR-physics-challenge)

Flow compensation challenge: 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ISMRM-MIT-CMR/CMR-physics-challenge/blob/master/ISMRM_final_challenge.ipynb)

### Submission [CLOSED]

**Deadline:** Wednesday 20th of May 2021, 11:59 am UTC <br/>
Once you open the submission link, you have **90 minutes** to submit your solution. 

**Template:** Please fill out the [template](template/ISMRM_MIT_CMR_PhysicsChallenge.potx) slide with 
- Abstract: Provide a short abstract (max. 150 words) about your solution
- Figure: Provide an overview figure depicting your final pulse sequence diagram as well as the simulated imaging result

**Submission:**
Once you open the submission link, you have **90 minutes** to submit your solution. <br/>
Please fill out the submission form and upload in this form:
- Template: Containing your abstract and overview figure
  - A short abstract on your solution
	- A plot of your sequence diagram
	- A figure containing: the original image, the reconstructed image with flow "scanned“ with the unmodified spGRE sequence, and the reconstructed image with flow 
- Results: Your Jupyter notebook as `*.ipynb` containing the modified pulse sequence code

### Solution
The solution will be discussed and presented in the [live session](Awards_Session.md) on Thursday, May 20 2021 at 18:00 - 19:00 UTC, and the challenge winners will be announced.

Example solution for flow compensation: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ISMRM-MIT-CMR/CMR-physics-challenge/blob/master/ISMRM_solution_flowcomp.ipynb)
