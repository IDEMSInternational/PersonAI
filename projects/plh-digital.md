---
id: plh-digital
name: PLH Digital
status: draft
---

# PLH Digital: parenting support for families with teenagers

## The product
*[to confirm] Michele asked for personas for "the parenting work for PLH". This file assumes that means **PLH Digital** as described in the 2020 decks in `sources/`. Since the scope change (2026-10-06), personas come after the product is known, so this must be confirmed before the set is shown to anyone outside the team. If it means a specific current product (e.g. ParentApp for Teens), the description below and the situations in the map should be checked against it.*

A digital form of the Parenting for Lifelong Health (PLH) for Teens programme, for families with adolescents in Sub-Saharan Africa. According to the 2020 user stories, it:
- delivers PLH parenting content as short, engaging sessions organised by topic: animated videos, illustrations, songs, little text
- sets home-practice tasks and reminders (to praise, to "take a pause" when upset, to do exercises), and lets people record what they did and what changed
- has activities and games for caregivers and teens to do together, and help with the family budget
- works on basic Android phones, offline, with little data
- is used **alongside facilitator-led PLH groups**, to catch up on missed sessions and keep going after the 14 sessions, **and on its own**
- gives programme data to M&E officers and researchers

## Who it serves
The 2020 deck names 14 potential users: caregivers of adolescents, adolescents, a facilitator, a community intermediary, and data users (M&E and research).

## Setting & constraints
- **Region:** Sub-Saharan Africa. The 2020 personas span 14 countries: DR Congo, Kenya, Nigeria, Sierra Leone, South Africa, Malawi, Ghana, Sudan, Senegal, Gabon, Angola, Niger, Zimbabwe, Rwanda. [to confirm] Which countries and partners are in scope now.
- **Phones:** mostly cheap Android, often given by someone else or borrowed; one feature phone; a few iPhones.
- **Data:** expensive and runs out; for some, WiFi only at work; power cuts take WiFi down.
- **Languages:** English, French, Portuguese and Arabic as official languages across the set, plus many local languages. [to confirm] Which are in scope.
- **Reading and eyesight:** some users read little or struggle with small text.
- **Safety:** violence at home appears in many of the stories, so safeguarding is part of the core.

## Links
- [Personas of 14 Potential Users of PLH Digital (13.03.2020)](../sources/Personas%20of%2014%20Potential%20Users%20of%20PLH%20Digital%2013.03.2020.docx)
- [User stories (13.03.2020)](../sources/USER%20STORIES%2013.03.2020.docx)
- [Vimbai Moyo slide](../sources/plh-persona-vimbai-moyo.png)
- [to confirm] Specs or repos of the current product(s), e.g. ParentApp for Teens or ParentText, if this map should cover them

## Coverage dimensions
1. **Role** relative to the system: caregiver, adolescent, facilitator, manager, intermediary, data user
2. **Relationship** to the teen: mother, father, grandparent / kinship carer, the teen, a teen who is also a parent
3. **Device, and who controls it**
4. **Connectivity & data cost**
5. **Reading, eyesight & language**
6. **Safety at home**

Families in the set (caregivers and teens):

| Persona | Relationship | Device (who controls it) | Data | Reading / eyesight / language | Setting | Safety at home |
|---|---|---|---|---|---|---|
| [Zawadi](../personas/zawadi-mwangi.md) | mother | Android from her employer | scarce, no WiFi | [to confirm]; Kenya | peri-urban | shouts; has hit her children |
| [Lindiwe](../personas/lindiwe-ngobeni.md) | grandmother, kinship carer | own cheap Android | WiFi lost in power cuts | poor eyesight; isiZulu/English [to confirm] | city | curses at grandchildren; granddaughter and an older man |
| [Aïssatou](../personas/aissatou-diop.md) | mother | two Androids, her own | [to confirm] | French/Wolof [to confirm] | city | screams; has hit her children |
| [Olusegun](../personas/olusegun-adeyemi.md) | father | own smartphone, likely iPhone [to confirm] | good [to confirm] | English | city | yells |
| [Hussein](../personas/hussein-ibrahim.md) | father | Nokia; borrows sons' Android | unreliable airtime | poor eyesight; Arabic [to confirm] | rural | whips his children |
| [Chibale](../personas/chibale-banda.md) | teen (14), kinship care | cheap Android; data money from uncle | little | simple language; Chichewa/English [to confirm] | city | conflict, no violence reported |
| [Efua](../personas/efua-mensah.md) | teen (17) | iPhone from an older boyfriend | runs out | English | city | conflict; relationship with a man in his late 20s |
| [Binta](../personas/binta-sesay.md) | teen (15), also a mother | Android from her baby's father | restaurant WiFi only | reads little; Krio/Temne/English [to confirm] | small town | rejected by family; may be told to leave |
| [Henri](../personas/henri-mba.md) | teen (17), also a father | cheap Android | little | French [to confirm] | town | breaks things; has hit his son's mother |
| [Diomo](../personas/diomo-kabongo.md) | young person (18) | cheap Android | little | out of school 3 years; Tshiluba/Lingala/French [to confirm] | town [to confirm] | fights; police custody |

## Persona map

### Building for now
| Persona | Role | Situation | Why they're in |
|---|---|---|---|
| [Zawadi Mwangi](../personas/zawadi-mwangi.md) | caregiver (mother) | Domestic worker away from home 4.30am–10pm, on her employer's phone with almost no data; shouts and hits when exhausted | The core PLH caregiver: loves her teens, shouts and hits when exhausted, has almost no time and little data. If it doesn't fit a 4.30am–10pm day on an employer's phone, it fails the people PLH most wants to reach. |
| [Lindiwe Ngobeni](../personas/lindiwe-ngobeni.md) | caregiver (grandmother, kinship carer) | Pensioner raising two orphaned teenage grandchildren, with poor eyesight and WiFi that goes in power cuts | Tests older users, eyesight, power cuts, and whether content only says "parents". |
| [Aïssatou Diop](../personas/aissatou-diop.md) | caregiver (mother) | French-speaking nurse and mother of three whose anger at her moody teens turns into screaming and hitting | The francophone caregiver. Tests French, faith fit, visible evidence, and help with her own anger. |
| [Olusegun Adeyemi](../personas/olusegun-adeyemi.md) | caregiver (father) | Well-off father who yells at his teens, and wants help in private rather than in a group | The only father in this group. Tests private, self-guided use (no group, username, no ads) and content that speaks to fathers. |
| [Chibale Banda](../personas/chibale-banda.md) | adolescent (14) | Orphaned 14-year-old in his uncle's family, with a cheap phone and data money that depends on his uncle | Younger teen in kinship care. Tests teen design, games with cousins, data cost, and privacy from his carers. |
| [Efua Mensah](../personas/efua-mensah.md) | adolescent (17) | 17-year-old in conflict with her religious parents over her future, on an iPhone from an older boyfriend | Older teen in high conflict with her parents. Tests teen privacy, negotiation rather than obedience, and iPhone support. |
| [Binta Sesay](../personas/binta-sesay.md) | adolescent (15), also a mother | 15-year-old mother, out of school, who reads little and has WiFi only at the restaurant where she works | The hardest teen to reach: out of school, reads little, WiFi only at work, phone from the baby's father. In as a teen in her father's family; her needs as a young mother are "not yet" (see Gaps). |
| [Vimbai Moyo](../personas/vimbai-moyo.md) | facilitator | Experienced facilitator whose voice tires during sessions, and who can't catch up families who miss one | Delivers PLH. The app must lighten her load (her voice, missed sessions, life after session 14), not add to it. |
| [Rehema Mushi](../personas/rehema-mushi.md) | programme manager | NGO manager of about 40 facilitators, deciding whether to adopt the app and how to keep it running | *[draft, new]* Decides whether an NGO adopts it and keeps it running. Tests full costs, safeguarding routes, facilitator workload, and what happens when the grant ends. |
| [Gahiji Uwimana](../personas/gahiji-uwimana.md) | data user (M&E) | M&E officer who needs routine monitoring data to keep programmes funded | Routine monitoring keeps programmes funded. In for monitoring only, not as a replacement for evaluation (his third ask), and only with data families agree to give. |

### Not building for, yet
| Persona | Role | Why not yet | What would change that |
|---|---|---|---|
| [Hussein Ibrahim](../personas/hussein-ibrahim.md) | caregiver (father) | Feature phone, and borrows his sons' Android; Arabic; rural Sudan, where the 2020 setting has since been overtaken by war [to confirm]. | A shared-phone mode (his own space on a family phone), audio-first content in Arabic, or an SMS/voice channel, plus a partner working with families in his situation. |
| [Diomo Kabongo](../personas/diomo-kabongo.md) | young person (18) | Above the PLH for Teens age range [to confirm: 10–17]. His needs (substance use, violence, police, work) go beyond parenting content. | A youth module, or referral links to youth, substance-use and employment services; a partner in DR Congo; French or Lingala. |
| [Henri Mba](../personas/henri-mba.md) | adolescent (17), also a father | At 17 he could turn up in a PLH for Teens family, but the content doesn't cover his main needs: young fatherhood, anger towards his son's mother, smoking and drinking. | Content for young parents, and a safeguarding route that covers partner violence. **Even now**, his safeguarding test question applies, because he may show up. |
| [Ana Lukamba](../personas/ana-lukamba.md) | intermediary (church leader) | Spreading PLH through community leaders and WhatsApp groups isn't part of the current model. In 2020 the team left open whether content should be shareable outside the app. | A decision on shareable, branded content; Portuguese; a defined "community champion" role with guidance on when to refer. |
| [Harouna Daouda](../personas/harouna-daouda.md) | data user (research) | Research needs (outcome tracking, comparisons across countries) go beyond routine monitoring, and need a study protocol, ethics approval and separate consent. | A specific study with its own protocol and consent flow; versioned content; documented, de-identified data export. |

### Deliberately not for
| Persona | Role | Why |
|---|---|---|
| [Samuel Kariuki](../personas/samuel-kariuki.md) | commercial partner (digital lending) | *[draft, new]* He would pay for families' data in exchange for their budget data and in-app loan offers. That solves a real problem (data cost) by turning families' money worries into a sales channel. Budget data, usage data and space in the app are not for sale. Any data sponsorship comes with no access in return. |
| [Nomvula Khumalo](../personas/nomvula-khumalo.md) | government social worker | *[draft, new]* She wants app activity as evidence about individual parents (court, case closure). If the app becomes a way to watch parents, they stop being honest in it, and some get judged on data that doesn't mean what it seems (a session missed because of a night shift). A safeguarding route *to* services like hers is wanted. A consent-based referral route *from* her could move her to "not yet". |

## Patterns across the set
*[draft] What the set says about the product as a whole.*

1. **Phones often belong to someone else.** Zawadi's came from her employer, Binta's from her baby's father, Efua's from her boyfriend; Hussein borrows his sons'. Lindiwe's granddaughter has one from an older man. Privacy (a PIN, a discreet name and notifications, nothing sensitive on screen) is a core need, not an extra.
2. **Violence is in most of the families.** Five involve physical violence (Zawadi, Aïssatou, Hussein, Henri, Diomo), and two more involve harsh words (Lindiwe, Olusegun). The "building for now" group needs a safeguarding and referral route now, not later.
3. **Privacy for teens pulls against data for adults.** Efua, Chibale and Binta need their own space. Gahiji, Harouna and Nomvula want more data. Every data field needs a reason a family would accept.
4. **Money comes up everywhere.** Six of the user stories ask for a budget tool. That makes budget data some of the most sensitive data the app could hold (see Samuel).
5. **Offline, low data, basic Android** appear in almost every user story. The exceptions are Efua's iPhone and Hussein's Nokia.

## Gaps
1. **Low-income fathers.** The only father in "building for now" is a wealthy banker; Hussein is out because of his phone. Either add a low-income father who would come to a PLH group, or bring Hussein in with a shared-phone mode.
2. **Rural families.** No one in "building for now" lives rurally.
3. **Younger adolescents (10–12) and their caregivers.** The youngest teen is Chibale, at 14.
4. **Both sides of one family.** There's no caregiver–teen pair (e.g. Efua and one of her parents), so we can't test how the app handles both sides of the same relationship.
5. **Less confident facilitators.** Vimbai is experienced. There's no new or volunteer facilitator with low digital confidence.
6. **Disability.** No caregiver or teen with a disability; the only access needs are Lindiwe's and Hussein's eyesight.
7. **Displacement.** No refugee or displaced family, though that may now describe families like Hussein's.
8. **Young parents.** Binta and Henri both have babies, which PLH for Teens doesn't cover.

## Still to confirm
- Which product this map is for (it now comes first: see "The product"), and which countries
- The PLH for Teens age range (10–17 assumed)
- Which languages are in scope
- Whether the new personas (Rehema, Samuel, Nomvula) and all [draft] stories ring true to people who know these settings
