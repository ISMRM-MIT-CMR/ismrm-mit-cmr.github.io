# Clinical Cardiovascular MR: How should we perform the examination

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
This tutorial shows how to conduct and plan a complete CMR examination. It will link the presented cardiovascular disease cases of session 1 to a clinically performed CMR protocol. It will also cover how to prepare a patient for a CMR scan, standard procedures and common mistakes, potential image artefacts together with their causes and how to minimize them. 

## Material
Further material can be obtained [here](encrypted.html)
