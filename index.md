{% include header.md %}

<div id="links">
  <ul>
    <li>
      <a href="https://twitter.com/alex_darby">Twitter</a>
    </li>
    <li>
      <a href="https://github.com/AlexDarby">GitHub</a>
    </li>
    <li>
        <a href="https://instagram.com/alex.darby">Instagram</a>
    </li>
    <li>
        <a href="https://www.linkedin.com/in/alex-darby/">LinkedIn</a>
    </li>
  </ul>
</div>

### Hi, I'm an Engineer, DevOps/Agile enthusiast based in Cardiff.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce mattis ullamcorper tincidunt. Fusce varius neque nisi, nec accumsan nisl rhoncus sit amet. Quisque dictum ante in ipsum facilisis, in mollis turpis pellentesque. Quisque interdum, nisl eget vehicula consequat, nulla metus egestas turpis, ac pretium orci ipsum vitae magna. Etiam tincidunt ante et enim sollicitudin vulputate. Nulla in tellus ullamcorper, mattis massa nec, pretium mi. Nulla mollis nisi sit amet urna mollis rhoncus. Fusce scelerisque, massa sed sodales dignissim, nisi arcu elementum est, vel tincidunt risus tortor faucibus nisi. Suspendisse suscipit, metus vel porttitor dictum, dolor urna lacinia odio, in condimentum odio velit ut est. Mauris aliquam facilisis interdum. Phasellus elementum congue purus, in lacinia elit sagittis non. Mauris eu quam scelerisque ipsum efficitur efficitur. Suspendisse neque nulla, vehicula vitae fermentum eget, hendrerit eget erat.




### Posts

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}

{% include footer.md %}