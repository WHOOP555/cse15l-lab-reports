# CSE 15L Lab Report 5: Find Command Line Options and Uses
## -name

**Example 1**

**Input Command:** `$ find written_2/travel_guides/berlitz2 -name "*.txt"`

**Output:** `written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Algarve-Intro.txt
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-History.txt
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-History.txt
written_2/travel_guides/berlitz2/Athens-Intro.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-History.txt
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
written_2/travel_guides/berlitz2/Barcelona-History.txt
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/Beijing-History.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2/travel_guides/berlitz2/Berlin-History.txt
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-history.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-History.txt
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-History.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Cancun-History.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
written_2/travel_guides/berlitz2/China-History.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-History.txt
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/CostaBlanca-History.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-History.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-History.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-History.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
written_2/travel_guides/berlitz2/NewOrleans-History.txt
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Poland-History.txt
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-History.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt`

**Example 2**

**Input Command:** `$ find written_2/travel_guides/berlitz2 -name "*-WhatToDo.txt"`

**Output:** `written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt`

In these examples, the -name command-line option ensures that the output returns the files that have the matching text in quotes from the respective files/directories.
This is useful because it easily allows the user to determine patterns between certain files in a directory and search for files with related names. Furthermore, -name can be used to search for a type of file as well, as the file extension can be a part of the file name pattern in the quotes.
*I found about this from asking OpenAI's chatGPT "what are some command line options and uses for find".*
***
## -type

Example 1

**Input Command:** `$ find written_2/ -type d`

**Output: ** `written_2/
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Rybczynski
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2`

**Example 2**

**Input Command:** `$ find written_2/non-fiction/OUP -type f`

**Output:** `written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt`

In these examples, the -type command-line option ensures that the output returns the type of output we are searching for within the file/directory we are finding in. For example, to find directories we would used -type d and to find files -type f.
This can be useful if one wants to ensure that they only find certain types of output (even links) when going through some directory.
*I found about this from asking OpenAI's chatGPT "what are some command line options and uses for find".*
***
## -size


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
*I found about this from asking OpenAI's chatGPT "what are some command line options and uses for find".*
***
## -print


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

*I found about this from asking OpenAI's chatGPT "what are some command line options and uses for find".*
