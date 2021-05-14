# Clinical Cardiovascular MR: What do we see and why do we need it?

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

This tutorial will cover basic cardiac anatomy and function, common cardiovascular diseases and cardiomyopathies as well as the clinical CMR protocols used for their diagnosis.
