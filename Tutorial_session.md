<img src="MIT_logo_small.jpg" height="80%" width="80%"/>

# ISMRM 2021 Member initiated tutorial: Cardiovascular MR - From Theory to Practice

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

## Overview
Cardiovascular magnetic resonance (CMR) has emerged as a clinically important technique for the assessment of cardiac anatomy, function, perfusion and viability. However, diversity and complexity of imaging and reconstruction methods pose some limitations to the widespread use of CMR. Therefore, it is necessary to bridge the gap between the clinical and scientific communities.
The tutorial at the ISMRM 2021 annual meeting on **Saturday 15th of May 2021, 16:00 to 20:30 UTC** will cover in five sessions different aspects of CMR:  
1. CMR methods for identifying cardiovascular disease with a case-based tutorial
2. Conduction and planning of a complete CMR exam
3. CMR pulse sequence building with a live computational MR physics tutorial
4. Machine learning for CMR image reconstruction with a live deep learning tutorial
5. Panel discussion on current challenges and future directions of CMR

Sessions 1 and 2 will provide a clinical background while sessions 3 and 4 cover state-of-the-art acquisition and reconstruction methods and current research developments including recent advances in the field of deep learning. Sessions 3 and 4 will host a code challenge for the audience to participate in.

Awards will be announced on **Thursday, 20 May 2021 at 18:00 - 19:00 UTC**.

## Target Audience
Physicians, radiographers, physicists, engineers, who wish to understand the main clinical applications of CMR, acquisition and reconstruction methods. The tutorial is suitable for beginners in the field and for more advanced users to refresh or deepen their understanding on different aspects of CMR.

## Educational objectives
* Understand basic cardiac anatomy, cardiovascular diseases, and its characterization by CMR and other diagnostic tools
* Describe the basic CMR examination and recognize the advantages and limitations of the technique
* Explain the basics of anatomical, functional, multi-multiparametric and quantitative imaging
* Explain the basics of deep learning-based methods for image reconstruction

## Sessions
[Tutorial session: Saturday, May 15 2021, 16:00 - 20:30 UTC](https://www.ismrm.org/21/program-files/T-04.htm)<br/>
[Awards session: Thursday, May 20 2021, 18:00 - 19:00 UTC](https://www.ismrm.org/21/program-files/T-31.htm)

### Organization/moderation
[Teresa Correia](https://www.ccmar.ualg.pt/users/tmcorreia) & [Thomas Küstner](http://www.midaslab.org/people.html)

### Speakers
1. Tevfik F. Ismail, MD, PhD, FSCMR<br/>
King's College London, United Kingdom<br/>
**[Clinical Cardiovascular MR: What do we see and why do we need it?](Talk1.md)**
2. Wendy Strugnell, BSc (MIT), FSMRT<br/>
Queensland X-Ray, Mater Hospital Brisbane, Australia<br/>
**[Clinical Cardiovascular MR: How should we perform the examination](Talk2.md)**
3. Sebastian Weingärtner, PhD<br/>
Delft University of Technology, Netherlands<br/>
**[The Physics behind Cardiovascular MR & Challenge](CMR-physics-challenge.md)**
4. Kerstin Hammernik, PhD<br/>
Technical University of Munich, Germany<br/>
**[Recent Advances in Machine Learning for CMR & Challenge](CMR-deep-learning-reconstruction-challenge.md)**
