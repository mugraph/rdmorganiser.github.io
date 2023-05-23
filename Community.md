---
layout: page

key: rdmo-arge
lang: de
---

# RDMO Arbeitsgemeinschaft 

Mit dem Ende der DFG-Förderung für RDMO im Herbst 2020 hat sich die Arbeitsgemeinschaft RDMO bei der Nutzerversammlung am 07.10.2020 gegründet. Sie basiert auf der freiwilligen Mitarbeit von Institutionen und Individuen, um die Open Source Software RDMO weiterhin nutzbar zu halten und weiterzuentwickeln.
Mit Unterzeichnung des [Memorandum of Understanding (MoU)]({{ site.baseurl}}/docs/Memorandum-of-Understanding-RDMO.pdf) haben sie ihre Unterstützung bekundet.

Die Organisationsstruktur mit verschiedenen Gremien soll diese Entwicklung tragen und ist im MoU detailliert ausgeführt.

## Steuerungsgruppe

Die RDMO-Arbeitsgemeinschaft wird von einer Steuerungsgruppe (SG) geleitet. Die Vertreter\*innen der Steuerungsgruppe werden durch die Mitglieder auf der Mitgliederversammlung alle drei Jahre oder nach Bedarf neu gewählt.
Die SG wird die Richtung der Weiterentwicklung begleiten und die Abstimmungsprozesse für die Weiterentwicklung der Software und des Contents koordinieren. Die SG setzt sich aus mindestens fünf Personen zusammen. 

So erreichen Sie die Steuerungsgruppe: rdmo-steuerungsgruppe@listserv.dfn.de

{% for member in site.data.sg-group.current %}
<div class="team-member">
    <img src="{{ site.baseurl }}/{{ member.image}}" />
    <div class="team-member-info">
        {{ member.text.de | markdownify }}
    </div>
</div>
{% endfor %}


## Entwicklungsgruppe

Die technische Koordination und Weiterentwicklung von RDMO erfolgt durch eine Entwicklungsgruppe (EG). Neben einem Kern von langfristig engagierten
Entwickler\*innen, die die Entwicklung kontinuierlich vorantreiben, ist auch eine niedrigschwellige Beteiligung einer größeren Anzahl von Entwickler\*innen wünschenswert und möglich. Diese können z. B. projektgebunden zur Entwicklung beitragen.

So erreichen Sie die Entwicklungsgruppe: [Slack](https://rdmo.slack.com/archives/CFRAZJ9LG)

{% for member in site.data.sw-group.current %}
<div class="team-member">
    <img src="{{ site.baseurl }}/{{ member.image}}" />
    <div class="team-member-info">
        {{ member.text.de | markdownify }}
    </div>
</div>
{% endfor %}


## Contentgruppe

Die Contentgruppe (CG) setzt sich aus Freiwilligen zusammen, die die inhaltliche Koordination und Weiterentwicklung von RDMO vorantreiben. Eine niedrigschwellige Beteiligung einer größeren Anzahl von Freiwilligen ist wünschenswert und möglich. Diese können z. B. projektgebunden zur Entwicklung beitragen.
Im Fokus der Arbeit stehen die Pflege und die kontrollierte Zusammenführung bestehender und neu generierter Inhalte wie beispielsweise Attribute oder Fragenkatalog-Templates. Es erfolgt eine Moderation und Begleitung der einzelnen Prozesse sowie Domänen-Anpassungen. Die CG dient dazu User Feedback einzusammeln und die allgemeine Usability vor dem Hintergrund des Feedbacks zu prüfen und ggf. zu verbessern.

So erreichen Sie die Contentgruppe: [E-Mail](rdmo-contentgruppe@listserv.dfn.de), [Slack](https://rdmo.slack.com/archives/C8B6VCKJ9)

{% for member in site.data.cg-group.current %}
<div class="team-member">
    <img src="{{ site.baseurl }}/{{ member.image}}" />
    <div class="team-member-info">
        {{ member.text.de | markdownify }}
    </div>
</div>
{% endfor %}


## Ad-Hoc-Gruppen

Für spezielle Aufgaben und Fragestellungen können aus dem Kreis der Mitglieder jederzeit weitere Arbeitsgruppen gebildet werden, die mit der Steuerungsgruppe abgestimmt werden.
Über die Weiterführung der Ad-Hoc-Gruppen entscheidet die Mitgliederversammlung.

## Mitgliederversammlung

Die Mitgliederversammlung der RDMO-Arbeitsgemeinschaft stellt die Gesamtheit aller Mitglieder dar. Anwender und weitere Interessenten können an der Mitgliederversammlung teilnehmen. Die Mitglieder wählen die Vertreter\*innen in der Steuerungsgruppe.
Die Mitgliederversammlung tritt je nach Bedarf mindestens aber einmal pro Jahr zusammen.


## Ehemalige Community-Mitglieder 

<details>
  <summary><u>Ehemalige Mitarbeiterinnen und Mitarbeiter</u></summary>
  {% for member in site.data.former %}
<div class="team-member">
    <img src="{{ site.baseurl }}/{{ member.image}}" />
    <div class="team-member-info">
        {{ member.text.de | markdownify }}
    </div>
</div>
{% endfor %}
</details>
