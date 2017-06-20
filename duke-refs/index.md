---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Duke-UNC Officials game-by-game since 03-04

#### Filter by a referee's first or last name

<pre class="huffman stilwata">
|     Name     | # of Games |
|:------------:|:----------:|
|   Karl Hess  |     10     |
| Bryan Kersey |      9     |
|  Roger Ayers |      7     |
|   Les Jones  |      7     |
</pre>

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th data-sortable="false">Box Score</th>
           <th >Location ↑↓</th>
           <th >Season ↑↓</th>
           <th data-sortable="false">Ref 1</th>
           <th data-sortable="false">Ref 2</th>
           <th data-sortable="false">Ref 3</th>
         </tr>
     </thead>

    <tbody>
	{% for duke in site.data.dukes %}
		<tr style="background-color: #{{ duke.style }};">
  			<td><a href="{{ duke.box }}" target="_blank">{{ duke.game }}</a></td>
  			<td>{{ duke.location }}</td> 
        <td>{{ duke.season }}</td> 
        <td>{{ duke.off1 }}</td> 
  			<td>{{ duke.off2 }}</td>
  			<td>{{ duke.off3 }}</td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


