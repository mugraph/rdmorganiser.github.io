---
layout: page

key: news
lang: en
---

# News

On this page we summarize our current activities.
To stay up to date, subscribe to our mailing list [rdmo@listserv.dfn.de](https://www.listserv.dfn.de/sympa/info/rdmo), follow us on [Twitter](https ://twitter.com/rdmorganiser), or chat with us on [Slack](https://rdmo.slack.com).
(Write an email to us: <a href="mailto:rdmo-team@listserv.dfn.de">rdmo-team@listserv.dfn.de</a> and we will invite you to Slack.) <br/>

{% for announcement in site.data.announcements.current %}
## Announcements:

<table style="width: 100%; border: 3px dotted red;">
  <tr>
    <th style="width: 20%; padding: 10px;"></th>
    <td style="width: 80%; padding: 10px;"></td>
  </tr>
  <tr>
    <th style="width: 20%; padding: 10px;">{{ announcement.date | markdownify }}</th>
    <td style="width: 80%; padding:10px;">{{ announcement.event.en | markdownify }}
    </td>
  </tr>
</table>
{% endfor %}

<br/>

The [RDMO working group]({{ site.baseurl }}/en/Community) was constituted with the event on October 7th, 2020. It calls on RDMO users to participate in further work on the basis of the [Memorandum of Understanding (MoU)]({{ site.baseurl}}/docs/Memorandum-of-Understanding-RDMO.pdf).
For connection information to the workshops and regular dates, please contact the RDMO working group or the responsible person. Interested people are welcome.

## Regular RDMO video conference dates
(Status: April 2023)


<table style="width: 100%; border:1px solid black;">
	<tr>
		<th style="width: 20%;"/>
		<th style="width: 45%; padding: 10px;">Fokus</th>
		<th style="width: 20%; padding: 10px;">Termin</th>
		<th style="width: 25%; padding: 10px;">Ansprechperson</th>
	</tr>
	{% for group in site.data.groups.current %}
	<tr>
		<td style="font-weight: bold; padding: 10px;">{{ group.name_en | markdownify }}</td>
		<td style="padding: 10px;">
			<ul>
				<li>{{ group.content_en1 | markdownify }}</li>
				<li>{{ group.content_en2 | markdownify }}</li>
			</ul>
		</td>
		<td style="padding: 10px;">{{ group.date_en | markdownify }}</td>
		<td style="padding: 10px;"><a href="{{ group.leader_mail }}">{{ group.leader | markdownify }}</a></td>
	</tr>
	{% endfor %}
	{% for group in site.data.groups.former %}
	<tr style="border:1px solid grey; border-bottom-right-radius: 15px; color:grey;">
		<td style="font-weight: bold; padding: 10px;">{{ group.name_en | markdownify }}</td>
		<td style="padding: 10px;">
			<ul>
				<li>{{ group.content_en1 | markdownify }}</li>
				<li>{{ group.content_en2 | markdownify }}</li>
			</ul>
		</td>
		<td style="padding: 10px;">{{ group.date_en | markdownify }}</td>
		<td style="padding: 10px;"><a href="{{ group.leader_mail }}">{{ group.leader | markdownify }}</a></td>
	</tr>
	{% endfor %}
</table>
