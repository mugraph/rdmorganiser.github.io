---
layout: page

key: news
lang: de
---

# Aktuelles

Auf dieser Seite fassen wir komprimiert unsere aktuellen Aktivitäten zusammen.
Um immer auf dem neuesten Stand zu bleiben, abonnieren Sie unsere Mailingliste [rdmo@listserv.dfn.de](https://www.listserv.dfn.de/sympa/info/rdmo), folgen uns auf [Twitter](https://twitter.com/rdmorganiser), oder diskutieren mit uns auf [Slack](https://rdmo.slack.com).
(Schreiben Sie eine E-Mail an uns: <a href="mailto:rdmo-team@listserv.dfn.de">rdmo-team@listserv.dfn.de</a> und wir laden Sie zu Slack ein.)<br/>

{% for announcement in site.data.announcements.current %}
## Ankündigung:

<table style="width: 100%; border: 3px dotted red;">
  <tr>
    <th style="width: 20%; padding: 10px;"></th>
    <td style="width: 80%; padding: 10px;"></td>
  </tr>
  <tr>
    <th style="width: 20%; padding: 10px;">{{ announcement.date | markdownify }}</th>
    <td style="width: 80%; padding:10px;">{{ announcement.event.de | markdownify }}
    </td>
  </tr>
</table>
{% endfor %}
<br/>

Die [Arbeitsgemeinschaft RDMO]({{ site.baseurl }}/Community) hat sich mit der Veranstaltung am 07.10.2020 konstituiert. Sie ruft die Anwender von RDMO auf, sich auf der Grundlage des [Memorandum of Understanding (MoU)]({{ site.baseurl}}/docs/Memorandum-of-Understanding-RDMO.pdf) an der Weiterarbeit zu beteiligen.
Für die Verbindungsinformation zu den Workshops und regulären Terminen bitte die RDMO-Arbeitsgemeinschaft oder die jeweiligen Verantwortlichen kontaktieren. Interessierte sind herzlich willkommen.


## Reguläre RDMO-Videokonferenz-Termine
(Stand: April 2023)

<table style="width: 100%; border:1px solid black;">
	<tr>
		<th style="width: 20%;"/>
		<th style="width: 45%; padding: 10px;">Fokus</th>
		<th style="width: 20%; padding: 10px;">Termin</th>
		<th style="width: 25%; padding: 10px;">Ansprechperson</th>
	</tr>
	{% for group in site.data.groups.current %}
	<tr>
		<td style="font-weight: bold; padding: 10px;">{{ group.name_de | markdownify }}</td>
		<td style="padding: 10px;">
			<ul>
				<li>{{ group.content_de1 | markdownify }}</li>
				<li>{{ group.content_de2 | markdownify }}</li>
			</ul>
		</td>
		<td style="padding: 10px;">{{ group.date_de | markdownify }}</td>
		<td style="padding: 10px;"><a href="{{ group.leader_mail }}">{{ group.leader }}</a></td>
	</tr>
	{% endfor %}
	{% for group in site.data.groups.former %}
	<tr style="border:1px solid grey; border-bottom-right-radius: 15px; color:grey;">
		<td style="font-weight: bold; padding: 10px;">{{ group.name_de | markdownify }}</td>
		<td style="padding: 10px;">
			<ul>
				<li>{{ group.content_de1 | markdownify }}</li>
				<li>{{ group.content_de2 | markdownify }}</li>
			</ul>
		</td>
		<td style="padding: 10px;">{{ group.date_de | markdownify }}</td>
		<td style="padding: 10px;"><a href="{{ group.leader_mail }}">{{ group.leader }}</a></td>
	</tr>
	{% endfor %}
</table>




