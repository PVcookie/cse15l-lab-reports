## Lab Report 3 - Researching Commands

# 1. grep -c
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

I chose the grep command. The first that I chose to do was -c. -c searches and displays the number of times a string appears 
in a file.

The first command is:

`grep -c 'Paris' travel_guides/*/*.txt`

output is:

`travel_guides/berlitz1/HandRHawaii.txt:0
travel_guides/berlitz1/HandRHongKong.txt:0
travel_guides/berlitz1/HandRIbiza.txt:0
travel_guides/berlitz1/HandRIsrael.txt:1
travel_guides/berlitz1/HandRIstanbul.txt:0
travel_guides/berlitz1/HandRJamaica.txt:0
travel_guides/berlitz1/HandRJerusalem.txt:0
travel_guides/berlitz1/HandRLakeDistrict.txt:0
travel_guides/berlitz1/HandRLasVegas.txt:0
travel_guides/berlitz1/HandRLisbon.txt:0
travel_guides/berlitz1/HandRLosAngeles.txt:0
travel_guides/berlitz1/HandRMadeira.txt:0
travel_guides/berlitz1/HandRMadrid.txt:1
travel_guides/berlitz1/HandRMallorca.txt:0
travel_guides/berlitz1/HistoryDublin.txt:0
travel_guides/berlitz1/HistoryEdinburgh.txt:0
travel_guides/berlitz1/HistoryEgypt.txt:0
travel_guides/berlitz1/HistoryFrance.txt:22
travel_guides/berlitz1/HistoryFWI.txt:5
travel_guides/berlitz1/HistoryGreek.txt:0
travel_guides/berlitz1/HistoryHawaii.txt:0
travel_guides/berlitz1/HistoryHongKong.txt:0
travel_guides/berlitz1/HistoryIbiza.txt:0
travel_guides/berlitz1/HistoryIndia.txt:0
travel_guides/berlitz1/HistoryIsrael.txt:0
travel_guides/berlitz1/HistoryIstanbul.txt:0
travel_guides/berlitz1/HistoryItaly.txt:0
travel_guides/berlitz1/HistoryJamaica.txt:0
travel_guides/berlitz1/HistoryJapan.txt:0
travel_guides/berlitz1/HistoryJerusalem.txt:0
travel_guides/berlitz1/HistoryLakeDistrict.txt:0
travel_guides/berlitz1/HistoryLasVegas.txt:0
travel_guides/berlitz1/HistoryMadeira.txt:0
travel_guides/berlitz1/HistoryMadrid.txt:0
travel_guides/berlitz1/HistoryMalaysia.txt:0
travel_guides/berlitz1/HistoryMallorca.txt:0
travel_guides/berlitz1/IntroDublin.txt:0
travel_guides/berlitz1/IntroEdinburgh.txt:0
travel_guides/berlitz1/IntroEgypt.txt:0
travel_guides/berlitz1/IntroFrance.txt:8
travel_guides/berlitz1/IntroFWI.txt:3
travel_guides/berlitz1/IntroGreek.txt:0
travel_guides/berlitz1/IntroHongKong.txt:0
travel_guides/berlitz1/IntroIbiza.txt:0
travel_guides/berlitz1/IntroIndia.txt:0
travel_guides/berlitz1/IntroIsrael.txt:0
travel_guides/berlitz1/IntroIstanbul.txt:0
travel_guides/berlitz1/IntroItaly.txt:0
travel_guides/berlitz1/IntroJamaica.txt:0
travel_guides/berlitz1/IntroJapan.txt:0
travel_guides/berlitz1/IntroJerusalem.txt:0
travel_guides/berlitz1/IntroLakeDistrict.txt:0
travel_guides/berlitz1/IntroLasVegas.txt:0
travel_guides/berlitz1/IntroLosAngeles.txt:0
travel_guides/berlitz1/IntroMadeira.txt:0
travel_guides/berlitz1/IntroMadrid.txt:1
travel_guides/berlitz1/IntroMalaysia.txt:0
travel_guides/berlitz1/IntroMallorca.txt:0
travel_guides/berlitz1/JungleMalaysia.txt:0
travel_guides/berlitz1/WhatToDublin.txt:0
travel_guides/berlitz1/WhatToEdinburgh.txt:0
travel_guides/berlitz1/WhatToEgypt.txt:0
travel_guides/berlitz1/WhatToFrance.txt:3
travel_guides/berlitz1/WhatToFWI.txt:2
travel_guides/berlitz1/WhatToGreek.txt:0
travel_guides/berlitz1/WhatToHawaii.txt:0
travel_guides/berlitz1/WhatToHongKong.txt:0
travel_guides/berlitz1/WhatToIbiza.txt:0
travel_guides/berlitz1/WhatToIndia.txt:0
travel_guides/berlitz1/WhatToIsrael.txt:0
travel_guides/berlitz1/WhatToIstanbul.txt:0
travel_guides/berlitz1/WhatToItaly.txt:0
travel_guides/berlitz1/WhatToJamaica.txt:4
travel_guides/berlitz1/WhatToJapan.txt:0
travel_guides/berlitz1/WhatToLakeDistrict.txt:1
travel_guides/berlitz1/WhatToLasVegas.txt:0
travel_guides/berlitz1/WhatToLosAngeles.txt:0
travel_guides/berlitz1/WhatToMadeira.txt:0
travel_guides/berlitz1/WhatToMalaysia.txt:0
travel_guides/berlitz1/WhatToMallorca.txt:0
travel_guides/berlitz1/WhereToDublin.txt:0
travel_guides/berlitz1/WhereToEdinburgh.txt:0
travel_guides/berlitz1/WhereToEgypt.txt:2
travel_guides/berlitz1/WhereToFrance.txt:81
travel_guides/berlitz1/WhereToFWI.txt:5
travel_guides/berlitz1/WhereToGreek.txt:2
travel_guides/berlitz1/WhereToHawaii.txt:0
travel_guides/berlitz1/WhereToHongKong.txt:0
travel_guides/berlitz1/WhereToIbiza.txt:0
travel_guides/berlitz1/WhereToIndia.txt:0
travel_guides/berlitz1/WhereToIsrael.txt:1
travel_guides/berlitz1/WhereToIstanbul.txt:1
travel_guides/berlitz1/WhereToItaly.txt:2
travel_guides/berlitz1/WhereToJapan.txt:0
travel_guides/berlitz1/WhereToJerusalem.txt:0
travel_guides/berlitz1/WhereToLakeDistrict.txt:3
travel_guides/berlitz1/WhereToLosAngeles.txt:1
travel_guides/berlitz1/WhereToMadeira.txt:0
travel_guides/berlitz1/WhereToMadrid.txt:3
travel_guides/berlitz1/WhereToMalaysia.txt:0
travel_guides/berlitz1/WhereToMallorca.txt:0
travel_guides/berlitz2/Algarve-History.txt:1
travel_guides/berlitz2/Algarve-Intro.txt:0
travel_guides/berlitz2/Algarve-WhatToDo.txt:1
travel_guides/berlitz2/Algarve-WhereToGo.txt:0
travel_guides/berlitz2/Amsterdam-History.txt:0
travel_guides/berlitz2/Amsterdam-Intro.txt:1
travel_guides/berlitz2/Amsterdam-WhatToDo.txt:1
travel_guides/berlitz2/Amsterdam-WhereToGo.txt:2
travel_guides/berlitz2/Athens-History.txt:1
travel_guides/berlitz2/Athens-Intro.txt:0
travel_guides/berlitz2/Athens-WhatToDo.txt:0
travel_guides/berlitz2/Athens-WhereToGo.txt:0
travel_guides/berlitz2/Bahamas-History.txt:0
travel_guides/berlitz2/Bahamas-Intro.txt:0
travel_guides/berlitz2/Bahamas-WhatToDo.txt:0
travel_guides/berlitz2/Bahamas-WhereToGo.txt:1
travel_guides/berlitz2/Bali-History.txt:0
travel_guides/berlitz2/Bali-WhatToDo.txt:0
travel_guides/berlitz2/Bali-WhereToGo.txt:0
travel_guides/berlitz2/Barcelona-History.txt:0
travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
travel_guides/berlitz2/Barcelona-WhereToGo.txt:2
travel_guides/berlitz2/Beijing-History.txt:0
travel_guides/berlitz2/Beijing-WhatToDo.txt:0
travel_guides/berlitz2/Beijing-WhereToGo.txt:0
travel_guides/berlitz2/Berlin-History.txt:2
travel_guides/berlitz2/Berlin-WhatToDo.txt:0
travel_guides/berlitz2/Berlin-WhereToGo.txt:3
travel_guides/berlitz2/Bermuda-history.txt:0
travel_guides/berlitz2/Bermuda-WhatToDo.txt:7
travel_guides/berlitz2/Bermuda-WhereToGo.txt:4
travel_guides/berlitz2/Boston-WhereToGo.txt:1
travel_guides/berlitz2/Budapest-History.txt:0
travel_guides/berlitz2/Budapest-WhatToDo.txt:2
travel_guides/berlitz2/Budapest-WhereoGo.txt:3
travel_guides/berlitz2/California-History.txt:0
travel_guides/berlitz2/California-WhatToDo.txt:0
travel_guides/berlitz2/California-WhereToGo.txt:0
travel_guides/berlitz2/Canada-History.txt:1
travel_guides/berlitz2/Canada-WhereToGo.txt:3
travel_guides/berlitz2/CanaryIslands-History.txt:0
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:0
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:1
travel_guides/berlitz2/Cancun-History.txt:0
travel_guides/berlitz2/Cancun-WhatToDo.txt:0
travel_guides/berlitz2/Cancun-WhereToGo.txt:1
travel_guides/berlitz2/China-History.txt:0
travel_guides/berlitz2/China-WhatToDo.txt:0
travel_guides/berlitz2/China-WhereToGo.txt:0
travel_guides/berlitz2/CostaBlanca-History.txt:0
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:0
travel_guides/berlitz2/Costa-History.txt:0
travel_guides/berlitz2/Costa-WhatToDo.txt:0
travel_guides/berlitz2/Costa-WhereToGo.txt:0
travel_guides/berlitz2/Crete-History.txt:0
travel_guides/berlitz2/Crete-WhatToDo.txt:0
travel_guides/berlitz2/Crete-WhereToGo.txt:0
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:1
travel_guides/berlitz2/Cuba-History.txt:0
travel_guides/berlitz2/Cuba-WhatToDo.txt:2
travel_guides/berlitz2/Cuba-WhereToGo.txt:0
travel_guides/berlitz2/Nepal-History.txt:0
travel_guides/berlitz2/Nepal-WhatToDo.txt:0
travel_guides/berlitz2/Nepal-WhereToGo.txt:0
travel_guides/berlitz2/NewOrleans-History.txt:0
travel_guides/berlitz2/Paris-WhatToDo.txt:14
travel_guides/berlitz2/Paris-WhereToGo.txt:44
travel_guides/berlitz2/Poland-History.txt:0
travel_guides/berlitz2/Poland-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-History.txt:0
travel_guides/berlitz2/Portugal-WhatToDo.txt:0
travel_guides/berlitz2/Portugal-WhereToGo.txt:0
travel_guides/berlitz2/PuertoRico-History.txt:1
travel_guides/berlitz2/PuertoRico-WhatToDo.txt:0
travel_guides/berlitz2/PuertoRico-WhereToGo.txt:0
travel_guides/berlitz2/Vallarta-History.txt:0
travel_guides/berlitz2/Vallarta-WhatToDo.txt:0
travel_guides/berlitz2/Vallarta-WhereToGo.txt:0`

It searches through all the .txt files in travel-guides and searches for the amount of times the string "Paris" appears in each file.
This is useful for word counting and data collection.

The second command:
`grep -c 'info' non-fiction/OUP/Abernathy/ch1.txt`

The output:

`18`

This one searches through a specific .txt file and searches for the amount of times the string "info" appears. This is useful for the same
reason as the previous command.

# 2. grep -h
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

The second command I chose was grep -h. It displays the lines that have a specific string, but not the file name.
For example, if added onto the first example from the previous command you get:

input:

`grep -h -c 'Paris' travel_guides/*/*.txt`

output:

    `
    
    0
    0
    0
    1
    0
    0
    0
    0
    0
    0
    0
    0
    1
    0
    0
    0
    0
    22
    5
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    8
    3
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    1
    0
    0
    0
    0
    0
    0
    3
    2
    0
    0
    0
    0
    0
    0
    0
    0
    4
    0
    1
    0
    0
    0
    0
    0
    0
    0
    2
    81
    5
    2
    0
    0
    0
    0
    1
    1
    2
    0
    0
    3
    1
    0
    3
    0
    0
    1
    0
    1
    0
    0
    1
    1
    2
    1
    0
    0
    0
    0
    0
    0
    1
    0
    0
    0
    0
    0
    2
    0
    0
    0
    2
    0
    3
    0
    7
    4
    1
    0
    2
    3
    0
    0
    0
    1
    3
    0
    0
    1
    0
    0
    1
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    0
    1
    0
    2
    0
    0
    0
    0
    0
    14
    44
    0
    0
    0
    0
    0
    1
    0
    0
    0
    0
    0
    
    `


-h caused the names of the files to be omitted and so it now only shows the count instead. This is useful for when you want to count
how many times a word appears, but you don't care about the file names.

Another example of using -h:
`grep -h 'info' non-fiction/OUP/Abernathy/ch1.txt`

output:

`Fifty years later, it is hard to imagine a retailer—be it a high-end department store, mass merchandiser, or catalog service—limiting an individual customer’s clothing purchase. Retailers collect detailed point-of-sales information that reflects the real-time demand for goods by consumers. Through new computer systems, they share this information with suppliers who, in turn, can ship orders within days to automated distribution centers. The contemporary equivalent of Bond Stores now has a much better chance of avoiding stock-outs of popular items and the inventory gluts that lead to costly markdowns. By the same token, the overall risk associated with fickle consumers, numerous selling seasons, and segmented markets—along with fierce overseas competition—has currently made this a tough arena for American retailers and manufacturers.
The transformation of U.S. clothing and textile manufacturing is very much still in progress and has by no means been successful for every company; but these industries have entered a renaissance of sorts, one that reflects new information technologies and management practices as well as the new economics of international trade. This book describes what has happened since the postwar era in three 
related industries—retail, apparel, and textiles—and what such companies must do to improve performance. We cover the histories of these industries, including the information technologies that have transformed these enterprises, manufacturing processes, inventory management, the new role of logistics, and global trade implications and policies.
Supply channels are not new, of course; for centuries, fabric-makers have sold their wares to those 
who cut and sew garments. But, until recently, most channels in the textile and apparel industries have been characterized by arm’s-length relationships among relatively autonomous firms. It is only since the mid-1980s that a number of market and technological changes have encouraged companies to enhance the links among different stages of production and distribution. Indeed, retailers like Wal-Mart Stores, Kmart Corporation, and Dillard’s Inc. have been the driving forces behind changes in manufacturing and logistics systems in a way that was unheard of in Bond Stores’ time. For instance, entrepreneur Sam Walton built a retail juggernaut that began with thirty-nine Wal-Mart stores in 1971 and grew to almost three thousand by 1996. He did so by insisting that suppliers implement information technologies for exchanging sales data, adopt standards for product labeling, and use modern methods of material handling that assured customers a variety of products at low prices.
In many respects, our findings defy the conventional wisdom. When we began our research, we were advised by American industry participants to establish better performance measures—for example, how many minutes does it take to make a shirt? The traditional view holds that because manufacturing performance is determined by the labor time required to produce an item, then what applies to cars, for example, can also apply to clothing; therefore, U.S. apparel manufacturers might be able to save themselves by improving assembly operations.3 Yet after years of studying hundreds of American apparel firms, we have found that direct labor content is not the primary issue. The companies that have adopted new information systems and management practices, participating in a well-integrated channel, are the ones with the strongest performance today—not those that have simply improved assembly operations.
As shown in later chapters, manufacturers that invest in advanced information technologies and use them to change their methods of planning and production can significantly reduce the amount of inventory they hold, thereby reducing the need to mark down or write off unsold products at the end of a season. These manufacturers also earn twice as much in profits than suppliers that continue to operate along traditional lines. Yet the distinguishing feature of such high performers is not their success in shaving off labor costs in the assembly room; it is their effort in changing basic aspects of 
the way they manage their enterprises.
Although it is true that the American apparel industry could have given up in the early 1990s, with 
only distribution centers and designers remaining in this country, it did not. Instead, manufacturers have developed, or have been compelled to develop, a competitive service for retailers; best practice American producers can now deliver orders with just a few days’ notice, something overseas suppliers have difficulty achieving. These U.S. firms do so through electronic data interchange (EDI), automated distribution centers, and sophisticated inventory management—a triumph of information technology, speed, and flexibility over low labor rates.
Proposition 1:  The retail, apparel, and textile sectors are increasingly linked as a channel through information and distribution relationships.
But, as we have already emphasized, this is not the real world of apparel today. At its most fundamental level, the channel perspective reflects a revolution in retail practices. These practices have 
resulted in the integration of enterprises at all stages of the distribution and production chain, because of the infusion of real-time information on consumer sales. Instead of gearing planning and production decisions to forecasts and guesses made months in advance of a selling season, firms now receive periodic ongoing orders based on actual consumer expenditures. And companies in transformed retail-apparel-textile channels have established a complex web of computer hardware and software, other technologies, and managerial practices that have blurred the traditional boundaries between retailers and suppliers.
Proposition 2:  For apparel manufacturers, the key to success is no longer solely price competition 
but the ability to introduce sophisticated information links, forecasting capabilities, and management systems.
Fortunately, clothing production today is more than a simple price/cost game. Successful apparel manufacturers must now focus on their capability to respond accurately and efficiently to the stringent demands placed on them by new retailing practices. This requires establishing systems to handle electronic, real-time orders, as well as creating management and information systems capable of using incoming information to forecast, plan, track production, and manufacture (or source) products in a flexible and efficient manner. Needless to say, these new skills were not part of the management arsenal of traditional apparel firms.
Yet our research indicates that apparel leaders are building these new skills. Analysis of detailed 
industry data demonstrates that there have been substantial increases in apparel suppliers’ investments in information technologies, distribution systems, and other associated services during the same period that new types of retailing practices emerged. In addition, we have found that those firms under greatest pressure by innovative retailers have been the most likely to make such investments, as well as to invest in innovations in other stages of manufacturing. Most important, apparel-makers 
that have invested in major innovations to collect and use information perform much better than those that have done little to innovate production beyond providing basic information links to retailers.
Yet here the conventional wisdom misses other significant measures of performance. Managers in well-integrated channels pay attention to inventory costs, inventory replenishment practices, information reliability, and time to market rather than the traditional direct costs of labor and materials alone. In fact, competitive performance is already being driven less by how a company manages its assembly operations and more by how it manages the logistics of its operations as a whole. Our study shows that an apparel manufacturer can still be successful with a traditionally organized sewing room; a firm with innovative and productive assembly operations, on the other hand, may not be competitively viable if it has not invested in information links with retailers and other changes in management 
practices.
Apparel manufacturers are not the only ones learning this lesson the hard way. The emphasis on labor productivity that has preoccupied practitioners and analysts in many industries—such as the total labor minutes required to assemble a car—no longer makes as much sense now that information technology has revolutionized retailing in many product segments. For instance, the current labor costs associated with assembly constitute 40 percent of the final cost of a car. In contrast, distribution-related costs—those associated with the traditional structure of automobile retailing—constitute anywhere between 15 and 34 percent of final cost.30 It is little wonder that car companies are currently in the throes of radically restructuring their method of automobile distribution.
Apparel, textile, and fiber firms and retailers have recently joined to launch the Quick Response Program, designed to improve information flow, standardize recording systems, and improve turnaround time throughout the system.... The program could be an important boon to productivity and competitiveness.... Will Quick Response succeed? According to industry experts, that depends on whether it diffuses down to the high-fashion, quick turnaround segments of the industry or, like much new technology in this industry, is adapted to suit the needs of firms still committed to mass production.31     
Basic and fashion-basic apparel categories now constitute the lion’s share of industry sales, accounting for approximately 72 percent of all shipments.32 This implies that a far larger portion of the 
industry may be viable in the long run than the part that could be saved by “quick response” at the 
fashion end.33 Bear in mind, however, that this viability depends on manufacturers using information to plan and execute production in a more sophisticated manner than usual for this and other industries.
A Stitch in Time concludes with a look at the many factors shaping today’s retail-apparel-textile channel—from the complex management challenges facing suppliers to labor standards and macroeconomic policy. Chapter 13 (“The Global Marketplace”) reviews trends in U.S. imports and exports of apparel and textiles, including information on trade by countries and specific products. It then connects these trends to changing trade policies, emphasizing the growing regionalization of trade flows in different parts of the world. Chapter 14 (“Suppliers in a Lean World”) examines our survey results from 
another angle, evaluating firm performance in an integrated channel. Here we highlight the importance of combining information technologies, manufacturing innovations, and new methods of management to respond to lean retailing demands.
Finally, Chapter 15 (“Information-Integrated Channels”) touches on a number of public policy issues 
raised by our findings. These include what can be done about the continuing problem of sweatshops, the new international economics of trade, and the effect of information integration on the business cycle and consumer prices at the macroeconomic level. Last but not least, we take a realistic look at the competitive future of the U.S. retail, apparel, and textile industries.
The information-integrated channel, with its emphasis on time and product perishability, is the basis for our cautiously optimistic—and unconventional—outlook. Even more important, the forces examined in this book provide a glimpse into processes reshaping a considerable portion of the economy. Consumers no longer line up for a special suit at a store like Bond Stores; they also expect an ever more “fashionable” array of cereal products, computers, and automobiles. As the next chapter shows, the changes now under way have their roots in new technologies, just as technical advances in transportation and communication shifted the industrial landscape at the end of the last century.`

Here it showed every single line where "info" appeared. This is useful if you wanna know the conteext of where the string
appears and you already know the file you're searching.

# 3. grep -w
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

This command checks for the whole word, not just substrings. So for example if I searched for "talk" it would return the lines where
"talk" appeared, but not words like "talked" or "talks".

First example which returns nothing:

`grep -w 'info' non-fiction/OUP/Abernathy/ch1.txt
`

output:
nothing

It returned nothing because there were no lines in that file with just the full word "info".

Second example:

`grep -w  'sew' non-fiction/OUP/Abernathy/ch9.txt`

output:

`Whether the apparel item is casual or formal, the stitching in the garment must accomplish one or more of the following objectives. The primary reason to sew, of course, is to join individual pattern 
pieces. The second objective is to leave no raw edge of fabric to unravel. This feature is sometimes combined with the joining operation, as in the “felled seaming” on the inseam of jeans or the sleeve seam in men’s dress shirts. The felled seam was first used in work clothing because of its strength and has since migrated to other apparel items because of its visible stitch pattern. Decorative stitching is the third objective of sewing. In the felled seams of shirts and jeans, for example, the 
visible stitches might be of a color designed to decorate the garment.3 No matter which stitch pattern is being used or which seaming operation carried out, the sewing machine operator must guide one 
or more pieces of cloth together through the machine. That is the basis of modern sewing operations 
in manufacturing facilities.`

This command is useful because it can help search for more specific strings as opposed to returning every single line or word that contains
the string you are searching for

# 4. grep -o
Source: [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

This command displays only the matched string.

Example 1:
`grep -o 'info' non-fiction/OUP/Abernathy/ch1.txt`

output:

    `
    
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info
    info

    `
This is useful for just looking at how many times a string appears in a file.

You can combine -o with -c to give you the count of how many times the string appears in the file.

input:
`grep -o -c 'sew' non-fiction/OUP/Abernathy/ch9.txt`

output:
`32`

This is useful for counting the occurrences of a word.
