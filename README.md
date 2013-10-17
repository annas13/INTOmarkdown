#Open Source

* Hafrún Sigurðardóttir
* Anna Katrín Snorradóttir

## 1. Linux uppsetning

Í upphafi var valið  lið nr 2. í verkefninu. En það var gert því ég nennti ekki að hafa USB lykil (týnist bara). Þar var valið VirtualBox 4.2.18 fyrir Windows. Það tók enga stund að downloada. Því næst var downloadað Ubunta VirtualBox image, það var gert í gegnum síðuna http://virtualboxes.org/images/ubuntu/ skrollaði var lengst niður og valið næst síðasta linkinn sem leiddi svo áfram á síðuna sourceforge.net og þarf hófst downloadið. Það tók um það bil 15 mínutur. Það opnaðist reyndar skjal síðan sem vildi ekki opnast.. En áfram var haldið. Það þurfti að installa forriti sem heitir FinalTorrent til að geta opnað þetta image. En það virkaði síðan ekki. Svo endað var með að leita ofar í listann af link sem innihélt "Download" En nei, virkaði ekki heldur, nokkrar tilraunir til viðbótar voru reyndar. Og eftir ábendingu frá Daníel kennara var farið ofar í listann. Eftir tvö kvöld í rugli fengum við uppgefinn annan link sem gerir tölvuna dual boot. En það er að finna hér: http://www.ubuntu.com/download/desktop/windows-installer , þetta tók örfáar mínutur, tölvan endurræstir og draumar fóru að gerast. Það eina sem þarf að gera þegar startað er tölvunni er að velja á milli Windows 7 eða Ubunta, einfaldara gæti það ekki verið. 


## 2. Uppsetning á vim && git

Byrjað var á því að opna terminal gluggan og skrifa þar inn sudo apt-install vim, gekk eins og í sögu, bauð mér að updeita, sem ég gerði. Sama sagan var með Git. Tók enga stund og ekkert vesen. 


## 3. Unnið með Git (1. hluti)

Byrjað var á því að búa til aðgang fyrir alla meðlimi hópsins á síðunni www.github.com. Því næst var farið inn á síðuna  https://github.com/danielbsig/INTOPrufa og valið FORK, sú sem forkaði verkefnið þurfti síðan að bæta hinum hópmeðliminum við, en það var gert með því að fara í setting og í colloboaradors.  

Því næst var farið í að ná í SSH lykil, en fyrst þurfi að athuga hvort einn slíkur væri til staðar fyrir, en það var athugað með að fara í terminal og slá inn $ cd ~/.ssh og $ ls . Engir SSH lyklar voru fyrir svo farið var í skref tvö í að fá lykil. Áfram er unnið í terminal glugganum og því næst er slegin inn eftirfarandi texti: $ ssh-keygen -t rsa -C "netfang" og síðan $ ssh-add id-rsa en þá er beðið um skráar nafn og lykilorð. 

Þegar búið var að ná í SSH lykilinn var farið í að "clone" verkefnið. En það er gert með því að slá inn eftirfarandi í terminal gluggan git clone <url á forkaða verkefnið> 

Þriðja skrefið í þessu öllu saman var svo að breyta NIM.cpp skránni í vim. En það er gert með því að fara fyrst í insert mode, gert með að ýta á i, en ég breytti minni þannig að efst setti ég textann "Hafrún mun rusta þessum leik" smá hégómi, hver hefur ekki gott af því? En þegar búið er að breyta því er ýtt á esc til að fara í command mode og þaðan er hægt að ýta á :wq og þá kemst maður út úr vim. Því næst, til að athuga hvort allt hefði ekki breyst rétt gerði ég git commit -a -m "Mitt fyrsta git komment" þaðan til að sjá til þess að þetta fari í "respitory-ið á github er slegið inn git push origin master. 

Til að vera alveg viss um að mínar breytingar hafi átt sér stað fór ég aftur inná github síðuna https://github.com/hafrun13/INTOPrufa og opnaði þar "Mitt fyrsta git komment" og athugaði hvort breytingarnar hafi skilað sér, sem þær gerðu.

Annar meðlimur hópsins fór síðan inná central repository síðuna og copy-aði url slóðina. Opnaði terminal glugga og skrifaði þar inn git clone <url>. Opnaði vim NIM.cpp og gerði breytinguna "Nei ég mun rústa þessu í drasl!" vistaði breytinguna. Gekk úr skugga um að allar breytingar hafi átt sér stað í local repository með því að run-a eftirfarandi komment git commit -a -m "My first git commit". Eftir það submittaði ég breytingunum á repository github með eftirfarandi kommenti: git push origin master. Eftir það var skoðað central repository þar sem séð var að öll komment höfðu skilað sér.

Url að forkuðu repository: 
https://github.com/hafrun13/INTOPrufa.git  

## 4. Uppsettur hugbúnaður

Eftirfarandi forrit eru opin source og á tölvunum okkar:

Program 1. PuTTY, Licence = MIT License, url to the source: http://ryara.net/putty-url/ eða þetta http://opensource.org/licenses/ eða www.chiark.greenend.org.uk/~sgtatham/putty
Program 2. Code Blocks, Licence = GNU General Public License 3[1], url to the source: http://sourceforge.net/projects/codeblocks  
Program 3. VLC media player, Licence = GNU General Public License v2 or later and LGPL[5][6], url to the source: https://videolan.org/vlc/ 
Program 4. 7-zip, Licence = GNU LGPLv2.1+ with unRAR restriction[3]. url to source: http://www.7-zip.org/
Program 5. Texmaker, GNU GPL, Licence = http://www.xm1math.net/texmaker/

## 5. Unnið með Git (2. hluti)

Verkefnið í heild sinni gekk mjög vel. Það eina sem hægt er að segja að hafi valdið vandræðum var uppsetning á Linux. En þegar við höfðum fengið aðstoð gekk það mjög vel. Okkur fannst Ubuntu mjög flott og skemmtilegt að vinna á því. Við munum báðar nota það meira í komandi tíð. Verkefnið var áhugavert og krefjandi og vakti upp áhuga okkar á að vinna meir með github í framtíðinni.  

Hér þarf ekkert að gera annað en að setja niðurstöður úr 4. fyrstu liðunum inn í þetta skjal.
