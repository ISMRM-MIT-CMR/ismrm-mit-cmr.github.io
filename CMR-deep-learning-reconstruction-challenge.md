# CMR deep learning reconstruction tutorial and challenge

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

This tutorial will cover the basic building blocks needed for deep learning in CMR image reconstruction and analysis with a live deep learning tutorial.

### Code
[https://github.com/ISMRM-MIT-CMR/CMR-DL-challenge](https://github.com/ISMRM-MIT-CMR/CMR-DL-challenge)


## Challenge
Deep plug-and-play priors exploit the advantages of learning an advanced denoising scheme offline and plugging it into any optimization scheme to solve inverse problems, such as Magnetic Resonance Image Reconstruction.

The goal of this challenge is to find a way to reconstruct complex-valued MR images by using available denoisers. The plug-and-play prior challenge consists of two tasks:

1. Deploying a denoising model. If you plan to use available denoisers trained on real-valued images, you have to think about a way to apply them to the complex-valued images.
2. Definition of an optimization scheme. Inspiration can be found in the Suggested Reading section.

The code parts that have to be changed are marked with TODO.

The dataset `subject1.h5`, containing fully sampled k-space, can be used for quantitative and qualitative evaluation in the deployment phase. The results have to be generated for `subject2.h5`, which contains the undersampled k-space. The challenge will be evaluated quantitatively using the normalized root mean squared error (NRMSE), and based on the creativity and complexity to generate the solution.

We are looking forward to your creative submissions! Happy coding!

### Code
[https://github.com/ISMRM-MIT-CMR/CMR-DL-challenge](https://github.com/ISMRM-MIT-CMR/CMR-DL-challenge)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ISMRM-MIT-CMR/CMR-DL-challenge/blob/master/challenge_plug_and_play.ipynb)

### Submission [CLOSED]

**Deadline:** Wednesday 20th of May 2021, 11:59 am UTC

**Template:** Please fill out the [template](template/ISMRM_MIT_CMR_ReconChallenge.potx) slide with 
- Abstract: Provide a short abstract (max. 150 words) about your solution
- Figure: Provide an overview figure of your solution 

**Submission:**
Please fill out the submission form and upload in this form:
- Template: Containing your abstract and overview figure
- Results: Your Jupyter notebook as `*.ipynb` containing your solution 

  
### Solution
The solution will be discussed and presented in the [live session](Awards_Session.md) on Thursday, May 20 2021 at 18:00 - 19:00 UTC, and the challenge winners will be announced.

Exemplary solution code: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ISMRM-MIT-CMR/CMR-DL-challenge/blob/master/challenge_plug_and_play_sample_solution.ipynb)

