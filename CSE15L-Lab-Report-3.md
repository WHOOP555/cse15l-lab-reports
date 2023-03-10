# CSE 15L Lab Report 3: Grep Command-Line Options
## -c (or --count)

**Example 1**

**Input Command:** `$ grep "." --count written_2/non-fiction/OUP/Abernathy/ch1.txt`

**Output:** `74`

**Example 2**

**Input Command:** `$ grep -c "Bahamas" written_2/travel_guides/berlitz2/Bahamas-History.txt`

**Output:** `23`

In these examples, the -c command-line option ensures that the output returns the number of matching lines with the text in quotes (instead of the actual lines themselves).
This is useful because it easily allows the user to determine how many lines match a certain line of text: instead of having to save the output to a file and using `$ wc`, the user can simply use this.
*I found about this from asking OpenAI's chatGPT "what are some command line options for grep".*
***
## -n (or --line-number)

Example 1

**Input Command:** `$ grep -n "serene" written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt`

**Output: **`41:Cross the river via Magere Brug then travel one block north and take a left along the northern bank of the Herengracht Canal. Here you will get your first glimpse of the canal system which was built during Amsterdam’s Golden Age and revolutionized the city. During its time, probably the most sought after and expensive real estate in the world. Herengracht particularly has many beautiful houses which can really only be appreciated by an afternoon strolling by them (see box page 66). This part of town is still mostly residential and many houses have been converted into apartments for successful Amsterdammers. It is fascinating to peek inside at the ultra-modern interiors, which give a feel of the flair the Dutch seem to have for interior design.62:Although only a small square, and cut by so many tramlines that it is difficult to know which way to look, it has a very beautiful tower — Muntorren (Mint Tower). Originally a medieval gate guarding the entrance to the city, it was damaged by fire in 1619, and the clock tower was added by de Keyser during the renovations of 1620. In 1699 the carillon was installed and this still fills the air with its regular bell rounds. During the war with France in 1672, when Amsterdam had its supply of money cut off, the tower was transformed for a short time into the city mint, and the name has remained since that time.
94:Beside the Palace sits Nieuwe Kerk (New Church) built before the Royal Palace, but not the oldest church in the city, hence its name. The church has suffered several catastrophic fires during its history and was stripped of all its treasures during the Alteration. The pulpit is interesting since it is beautiful but extremely ornate for a Protestant place of worship.119:Just 5 km (2.75 miles) beyond Monnickendam is the community of Marken, one of the most beautiful villages in the Netherlands and home to a community of Calvinist Dutch whose traditions reach back hundreds of years. The older inhabitants of this close-knit community still wear traditional Dutch costume as everyday wear.`

**Example 2**

**Input Command:** `$ grep "Bali" -n written_2/travel_guides/berlitz2/Bali-History.txt`

**Output:** `6:Today’s Indonesians mainly descend from people who came from south China via the Malay peninsula and moved along the island chain to Java, Bali, Lombok, and beyond, from 3000 to 1000 b.c. Archaeological finds show that there was a flourishing Bronze Age culture in Bali and Lombok between about 1000 and 100 b.c. Trade and cultural exchanges with Southeast Asia had certainly begun by that period, and there were frequent contacts with India by a.d. 100. About this time, too, wet rice cultivation was introduced to Bali, changing the face of the countryside to its present appearance of rice paddy fields and terraces.
7:Indian traders and teachers brought Buddhism to Java. It had only a limited influence in Bali, however, where people continued in their ancient animist beliefs, worshipping the spirits of the mountains, rivers, and other natural forces.
8:Hinduism Comes to Bali
9:In the eighth and ninth centuries a.d., several Buddhist rulers in Java converted to Hinduism, along with their subjects. This time, many people in Bali followed suit, perhaps attracted by the complex Hindu mythology — the Balinese today still have a love of the old stories — and by the way their local gods could be housed easily in the crowded Hindu pantheon. Around 930, the kingdom of East Java conquered Bali and the conversion process accelerated. A mild form of the caste system and the concept of the Hindu trinity of Brahma, Shiva, and Vishnu were introduced. But Bali was no mere vassal state of Java. From 1019 to 1042, Airlangga, son of the Balinese king Udayana, ruled over East Java with the help of a Javanese princess, while his young brother acted as regent in Bali. During the 12th and 13th centuries, Bali was often independent.
10:A powerful Hindu empire named after its capital, Majapahit, united all of Java by 1320. The Majapahit general Gajah Mada reconquered Bali in 1343, and annexed a large part of the Indonesian archipelago. Hindu art and scholarship spread through the islands, but on most of the islands, this flowering was short-lived. With the death in 1389 of King Hayam Wurukin, its last great ruler, the empire of Majapahit began to decline.
11:Muslim traders and teachers had already started converting several of Java’s princes and people to Islam, especially in coastal areas, and in the 14th and 15th centuries the movement spread to the interior. By the year 1500, seeing their world breaking up, many Majapahit aristocrats, priests, and scholars fled to Bali, where their culture continued to flourish. Islam never gained a strong foothold in Bali, which was difficult to invade because of its many reefs and lack of harbors, and had few products to attract traders. The early 16th century also brought the first European ships to Indonesian waters, when the Portuguese came in search of spices and set up trading posts — though not on Bali.
12:In 1550 Bali was united under Batu Renggong, the formidable ruler known as Dewa Agung (god-king) of Gelgel, near Klungkung. His men even succeeded in turning back the tide of Islam for a short while, adding eastern Java and Lombok to his domains. During his rule, Balinese power, culture, and influence reached a peak, with a boom in temple building and the associated crafts of sculpture and woodcarving.
13:During the next 250 years, Bali’s rulers fell to squabbling among themselves and the island split into ten or more rajadoms. Bali’s contact with the Dutch was restricted to providing slaves — mainly Balinese who had broken the rajas’ laws or priests’ taboos — and soldiers for the army of the United Dutch East Indies Company (Vereenigde Oostindische Compagnie, or VOC). The company was the instrument of influence of the Netherlands until it went bankrupt in 1799 and was superseded by the government. Throughout the 18th century, Dutch influence and authority slowly spread across the Indonesian archipelago, but bypassed the relatively poor, unimportant island of Bali.
14:Between 1811 and 1817, during the Napoleonic Wars, Britain took control of Indonesia and seriously thought of staying once the wars were over. Britain’s administrator, Stamford Raffles, who was named Lieutenant Governor, even visited Bali, and may have had it in mind to build a trading station here. After the war, however, the British government decided to restore Dutch territory and interests — and Raffles found another site, the island and future port of Singapore.
16:Once re-established in Java, the Dutch attempted to increase their influence and also to prevent the Balinese from plundering ships wrecked off the coast (the Balinese considered shipwrecks to be gifts from the deities of the seas, and felt it would be insulting to refuse them). Following the looting of a ship in 1841, the Dutch decided to use force. Some 1,600 men, recruited mainly from other Indonesian islands, landed on the north coast in 1846 and burned Singaraja. Immediately, the Balinese rajas agreed to stop the plundering of wrecks, and to pay compensation for the 1841 incident, but it soon became clear that they had no intention of honoring the deal. In 1848 the Dutch landed a second military expedition in the north of Bali. Advancing inland to attack the Balinese base at Jagaraga, they were ambushed by a bigger but less well-armed force led by Jelantik, younger brother of the Raja of Bululeng. In spite of appalling losses, the Balinese won the day. The defeated Dutch invaders retreated in disorder to their ships, but the following year, a third Dutch military expedition, far stronger than its predecessors, landed near Singaraja. The northern rajadoms sued for peace; they were offered terms calling for them to disarm and submit to Dutch rule. The response of Jelantik was to fall back to Jagaraga and prepare to fight. This time the Balinese were overwhelmed and thousands were killed, some in a suicidal march towards enemy guns, a ritual death in battle known in the Balinese language as puputan. After a second Dutch landing at Padangbai Bay, the puputan ritual was repeated when the Raja of Karangasem and his family threw themselves on the enemy guns.
17:During the rest of the 19th century, the Dutch, using the rajas and other aristocrats as regents, took control over most of Bali, but their influence in the south remained limited. This was emphasized in 1904 when a ship wrecked off Sanur was plundered of its cargo. The Dutch demanded reparations for this act; the southern rajas refused. In 1906 a force of mainly Moluccan troops led by Dutch officers marched on Denpasar to enforce compliance. They found the place almost deserted, until suddenly the Raja of Badung, together with his family and hundreds of courtiers, emerged from the palace. On a signal from the raja, one of his priests stabbed him with a kris (knife), and then, pausing only to stab their children first, the rest of the royal party began a puputan, either killing themselves or running suicidally towards the enemy. When the dreadful scene was repeated by the Dewa Agung and his wives and followers in 1908 in front of the palace at Klungkung, the rajas’ resistance to Dutch rule was at an end.
18:The public in the Netherlands was appalled by these grisly events. From then on, Bali and the Balinese came to be looked on as unique — to be protected from the colonial treatment that had turned the other islands into plantations exploited for profit. Tourism was discouraged, although a few foreigners did make the journey and returned to the outside world with news of the island’s extraordinary culture. An American couple, Bob and Louise Koke, opened the first hotel on Kuta Beach in 1936; Louise G. Koke’s memoir, Our Hotel In Bali, provides an idyllic portrait of Bali’s first, tenuous endeavor at tourism from 1936 until the Japanese invasion in 1942.
19:During the 1920s and 1930s, Cokorde Gde Agung Sukawati, ruler of Ubud, extended a long Sukawati family tradition of patronizing talent and craftsmanship by hosting visiting Western artists, including the German painter, Walter Spies, who stayed for 14 years. Spies’ influence revolutionized painting in Bali, which had previously been one of the least inventive of Bali’s arts, bound by repetitive conventions. The Pita Maha school of young Western-influenced artists emerged (also influenced by the Dutch pastel-ist, Rudolf Bonnet), putting Ubud on the world map of contemporary art. Spies’ house and spring-fed swimming pool (now part of the Tjampuhan Hotel) were visited by Western artists, academics, musicians, and stars of theater and film. Deeply involved in Balinese culture, Spies himself choreographed the still-performed version of the most famous Balinese dance, the kecak, based on a story from the “Ramayana.” When Germany invaded Holland in 1940, Spies was interned as an enemy alien. He died in 1942, when a ship on which he was being transported to British Ceylon was torpedoed by the Japanese.
23:On Bali, in November, 1946, Indonesian nationalist fighters, led by Ngurah Rai, found themselves trapped by Dutch forces close to Marga, north of Tabenan. Outnumbered and outgunned, Ngurah Rai and all 96 of his followers were killed in what is regarded as Bali’s last puputan. Their sacrifice is commemorated by a monument and museum at the site, together with stones bearing the names of each of those who died on the island of Bali during the struggle for independence (see page 68).
29:The country’s limited foreign-exchange reserves were squandered on window-dressing projects, grand monuments, and stadiums to host the Asian Games of 1962, seen as part of a plan to bring Indonesia into the world spotlight. International travel agents were given a tour of the country, including a visit to Bali that coincided with an important Balinese ceremony in March 1963 at the so-called “mother temple” Besakih, on the slopes of the island’s highest mountain, Gunung Agung. Portentously, Gunung Agung, though long dormant, chose this particular moment to begin emitting smoke and firing rocks into the air, but the ceremony went ahead anyway, literally under a cloud. The official guests had scarcely left Bali when Gunung Agung exploded in what was the most violent eruption the island had seen in centuries. Lava flowed down its slopes, but despite the impressions conveyed by reporters (and by photographs seen in many books), it covered only a limited area. The chief instrument of destruction was the volcanic ash that showered down on the northern half of Bali, covering it with a layer 40 cm (15 inches) thick. Crops were wiped out; the rice terraces were devastated, and starvation threatened.
30:The ash fall also blocked rivers, but the dams it formed could not retain the waters for long. When they broke, torrents of mud and rock tore down the valleys and through the villages and towns along the river banks. The official death toll of 1,600 was a wild underestimate. The sky went black even over southern Bali, although Denpasar received only a sprinkling of ash.
32:On 30 September 1965, a group of army conspirators, who claimed they acted to prevent a possible coup against Sukarno, kidnapped and killed six army generals. In the following days, General Suharto, one of the most senior surviving commanders, isolated the conspirators and effectively seized power. The blame for the killings was pinned on the Communist Party, the PKI, which denied any involvement. A pogrom was then unleashed, first in Java and next in Bali, with widespread killings of suspected Communists. The Chinese minority, mainly shopkeepers, moneylenders, and other small businesspeople, were also a target. In common with the other immigrant groups, they had been compelled by law to display the flag of their country of origin, even if a century had passed since their ancestors had come to Indonesia. Throughout Indonesia, every Chinese business, marked by the flag of China, and associated in people’s minds with communism, was attacked. The numbers killed will never be known: in Bali alone the total casualties may have exceeded 60,000.
35:In the decades following, the economy stabilized as growing oil revenues fueled expansion. The Chinese community, backbone of the nation’s economy, carefully rebuilt its commercial interests, this time much less visibly. Tourism to Bali was seen as a money-spinner: the 1970s saw a rapid increase in the numbers of foreign visitors. During the 1980s, the authorities decided to develop a more up-market tourism on Bali. Nusa Dua was designated to become a huge tourist enclave where only large, luxury hotels would be built. To bring the necessary volume of visitor traffic to fill all the new rooms, Denpasar Airport’s runway was extended out into the sea to handle big airliners. During the next decade, Bali became one of the most prosperous places in the country. In order to help Balinese better prepare for new jobs in the tourism market, English language courses became mandatory in middle and secondary schools throughout the island.
36:The late 1990s were a period of disillusionment with the long-lived Suharto regime’s many failings and widespread corruption. As the Indonesian economy faltered, ethnic conflicts erupted in many parts of the country; even Lombok experienced a brief flare-up of violence against Christians and ethnic Chinese. But Bali, with its unique Hindu culture and its international, tourism-oriented outlook, has remained an island of stability throughout this unsettled period of Indonesian history.`

In these examples, the -n command-line option ensures that the output not only returns the lines with the matching text, but also returns the line number of them in the file.
This can be useful if one wants to know not only whether some text is within a file, but also what line it is in within that file.
*I found about this from asking OpenAI's chatGPT "what are some command line options for grep".*
***
## -r (or --recursive)


**Example 1**

**Input Command:** `$ grep -r "serenity" written_2`

**Output:** `written_2/travel_guides/berlitz1/WhereToFrance.txt:        serenity that is in itself as evocative as the remaining concrete
written_2/travel_guides/berlitz1/WhereToIndia.txt:        repose and serenity made from a delicate combination of
written_2/travel_guides/berlitz1/WhereToItaly.txt:        can appreciate the typical Venetian serenity even without understanding
written_2/travel_guides/berlitz1/WhereToJapan.txt:        the eyes half-closed in an expression of profound serenity. The statue    
written_2/travel_guides/berlitz1/WhereToJapan.txt:        on Sundays it offers all the serenity of rush hour at Kyoto’s garish      
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:After the salty flavor of Olhão and the rural serenity of Moncarapacho, the aristocratic bearings of Tavira, one of the true gems of the Algarve, may come as something of a surprise. One of the region’s most historic cities, its Moorish, Reconquista, and Renaissance roots are clearly visible.`

**Example 2**

**Input Command:** `$ grep "pleasure" -r written_2/travel_guides/berlitz1`

**Output:** `written_2/travel_guides/berlitz1/HistoryHawaii.txt:        pleasure. These Western ideas, which seemed to amuse Kamehameha, were
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:        find a place next to worldly pleasures. The Malay aristocracy preferred
written_2/travel_guides/berlitz1/IntroIndia.txt:        least, pleasure. At the center of the confrontation with the harsh
written_2/travel_guides/berlitz1/IntroJamaica.txt:        The recreational pleasures that ordinary islanders enjoy
written_2/travel_guides/berlitz1/JungleMalaysia.txt:        be a rare sensual pleasure. Sounds flood in from all sides: the buzz    
written_2/travel_guides/berlitz1/WhatToHongKong.txt:        licensed by the Hong Kong authorities can run pleasure boats in local
written_2/travel_guides/berlitz1/WhatToIbiza.txt:        one of the area’s pleasures. A cup of coffee buys you a ringside seat      
written_2/travel_guides/berlitz1/WhatToIndia.txt:        At least half the pleasure is in the bargaining. If you
written_2/travel_guides/berlitz1/WhatToIndia.txt:        bargain, there is real aesthetic pleasure in seeing, at the end of the     
written_2/travel_guides/berlitz1/WhatToItaly.txt:        Sardinia, and Sicily, swimming is a pleasure that requires a few words     
written_2/travel_guides/berlitz1/WhatToJamaica.txt:        few hippies left today, but the pleasures are still pretty earthy: it’s
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:        view and it will bring you years of pleasure.
written_2/travel_guides/berlitz1/WhereToDublin.txt:        series of pleasure gardens in the Italianate style in 1865, with
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:        Sailboats and small pleasure craft dock at Cramond, where
written_2/travel_guides/berlitz1/WhereToEgypt.txt:        One of the great pleasures of a trip to Aswan is taking a
written_2/travel_guides/berlitz1/WhereToFrance.txt:        One of the simplest pleasures here is the stunning view of
written_2/travel_guides/berlitz1/WhereToFrance.txt:        important pleasure of Provence is not the sightseeing but the
written_2/travel_guides/berlitz1/WhereToFrance.txt:        exploring Bourges in the evenings a pleasure. The cathedral in
written_2/travel_guides/berlitz1/WhereToHongKong.txt:        Browsing is a real pleasure in Macau’s main streets and
written_2/travel_guides/berlitz1/WhereToIndia.txt:        served as the General’s pleasure-palace, but it was to be the death of    
written_2/travel_guides/berlitz1/WhereToIndia.txt:        air here is sweet, cool, and clear, and the pleasure of the quaint and    
written_2/travel_guides/berlitz1/WhereToIndia.txt:        made their way to other lakes for duck-shoots or just for the pleasures   
written_2/travel_guides/berlitz1/WhereToIndia.txt:        (Hall of pleasure), with doors inlaid in ivory and sandalwood. Inside,    
written_2/travel_guides/berlitz1/WhereToIndia.txt:        A major part of the pleasure of Darjeeling is in getting
written_2/travel_guides/berlitz1/WhereToIsrael.txt:        region; pleasure cruisers run to Capernaeum and other places; and you    
written_2/travel_guides/berlitz1/WhereToIstanbul.txt:        promenades. Nearby is the Kültür Parkı, a huge, shady pleasure garden,
written_2/travel_guides/berlitz1/WhereToItaly.txt:        humid in most big cities, but some find an odd, ghostly pleasure in       
written_2/travel_guides/berlitz1/WhereToItaly.txt:        man who drew no distinction between the pleasures of mind and body. In    
written_2/travel_guides/berlitz1/WhereToItaly.txt:        culinary pleasures.
written_2/travel_guides/berlitz1/WhereToItaly.txt:        Half the pleasure of this lovely town dramatically perched
written_2/travel_guides/berlitz1/WhereToItaly.txt:        its pleasures before you even set foot inside the museums, churches,      
written_2/travel_guides/berlitz1/WhereToItaly.txt:        chief pleasure of the south, or Mezzogiorno, is the people, who are       
written_2/travel_guides/berlitz1/WhereToItaly.txt:        bundle of old bones and stones, but sheer pleasure for anyone even
written_2/travel_guides/berlitz1/WhereToItaly.txt:        precipice, said to be the last pleasure enjoyed by the emperor’s
written_2/travel_guides/berlitz1/WhereToItaly.txt:        pleasure among the exotic flowers and trees and Arab fountain of its      
written_2/travel_guides/berlitz1/WhereToJapan.txt:        tranquilizing pleasures provided within.
written_2/travel_guides/berlitz1/WhereToJapan.txt:        Here, business and pleasure are inextricably linked — and
written_2/travel_guides/berlitz1/WhereToJapan.txt:        you to soak up the heady atmosphere of pleasure and commerce that has     
written_2/travel_guides/berlitz1/WhereToJapan.txt:        ideal introduction to the pleasures of bathing Japanese-style, whether    
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:        great pleasure in his later years.
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        pleasure-seeker who goes with the flow. While there’s much to see    
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        A number of boat trips leave from the pleasure pier. These
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        pleasure, not least of all for the myriad brightly colored butterflies
written_2/travel_guides/berlitz1/WhereToMallorca.txt:        an all-purpose port for commercial, naval, and pleasure craft (there’s 
written_2/travel_guides/berlitz1/WhereToMallorca.txt:        where pleasure craft congregate near the ships’ chandlers, shops, and  
written_2/travel_guides/berlitz1/WhereToMallorca.txt:        curving inlet lined with fishing boats on one side and pleasure craft`

In these examples, the -r command-line option ensures that the grep commands recursively searches through the current directory and all its subdirectories, searching through the files within those directories checking for the outlined keyword in the file. 
This can be useful to search for certain text through an entire directory and/or subdirectory, instead of having to do so in multiple commands.
*I found about this from asking OpenAI's chatGPT "what are some command line options for grep".*
***
## -o (or --only-matching)


**Example 1**

**Input Command:** `$ grep -o "democracy" written_2/travel_guides/berlitz2/Athens-History.txt`

**Output:** `democracy
democracy
democracy
democracy`

**Example 2**

**Input Command:** `$ grep "gold" -o written_2/travel_guides/berlitz2/California-History.txt`

**Output:** `gold
gold
gold
gold
gold
gold
gold
gold
gold`

In these examples, the -o command-line option ensures that the output only shows the matching parts of a line instead of the entire line.
This can be useful if one wants to only print the parts of a file which have the matching text to the terminal, instead of the lines of entire text.

*I found about this from asking OpenAI's chatGPT "what are some command line options for grep".*
