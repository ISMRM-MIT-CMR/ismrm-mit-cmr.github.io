# Tutorial session

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

## Description
[Tutorial session: Saturday, May 15 2021, 16:00 - 20:30 UTC](https://www.ismrm.org/21/program-files/T-04.htm)

### Organization/moderation
[Teresa Correia](https://www.ccmar.ualg.pt/users/tmcorreia) & [Thomas Küstner](http://www.midaslab.org/people.html)

### Speakers
1. Tevfik F. Ismail, MD, PhD, FSCMR<br/>
King's College London, United Kingdom<br/>
<b>Clinical Cardiovascular MR: What do we see and why do we need it?</b>
2. Wendy Strugnell, BSc (MIT), FSMRT<br/>
Queensland X-Ray, Mater Hospital Brisbane, Australia<br/>
<b>Clinical CMR: How should we perform the examination</b>
3. Sebastian Weingärtner, PhD<br/>
Delft University of Technology, Netherlands<br/>
<b>The Physics behind Cardiovascular MR & Challenge</b>
4. Kerstin Hammernik, PhD<br/>
Technical University of Munich, Germany<br/>
<b>Recent Advances in Machine Learning for CMR & Challenge</b>
