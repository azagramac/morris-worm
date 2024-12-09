### Architecture

Floppy disk containing the source code for the Morris Worm, at the Computer History Museum
The worm's creator, Robert Tappan Morris, is the son of cryptographer Robert Morris, who worked at the NSA. A friend of Morris said that he created the worm simply to see if it could be done,[3] and released it from the Massachusetts Institute of Technology (MIT) in the hope of suggesting that its creator studied there, instead of Cornell. Clifford Stoll, author of The Cuckoo’s Egg, wrote that "Rumors have it that [Morris] worked with a friend or two at Harvard's computing department (Harvard student Paul Graham sent him mail asking for 'Any news on the brilliant project')".[5]

The worm exploited several vulnerabilities of targeted systems, including:

A hole in the debug mode of the Unix sendmail program
A buffer overflow or overrun hole in the finger network service
The transitive trust enabled by people setting up network logins with no password requirements via remote execution (rexec) with Remote Shell (rsh), termed rexec/rsh
The worm exploited weak passwords. Morris's exploits became generally obsolete due to decommissioning rsh (normally disabled on untrusted networks), fixes to sendmail and finger, widespread network filtering, and improved awareness of weak passwords.

Though Morris said that he did not intend for the worm to be actively destructive, instead seeking to merely highlight the weaknesses present in many networks of the time, a consequence of Morris's coding resulted in the worm being more damaging and spreadable than originally planned. It was initially programmed to check each computer to determine if the infection was already present, but Morris believed that some system administrators might counter this by instructing the computer to report a false positive. Instead, he programmed the worm to copy itself 14% of the time, regardless of the status of infection on the computer. This resulted in a computer potentially being infected multiple times, with each additional infection slowing the machine down to unusability. This had the same effect as a fork bomb, and crashed the computer several times.

The main body of the worm can infect only DEC VAX machines running 4BSD, alongside Sun-3 systems. A portable C "grappling hook" component of the worm was used to download the main body parts, and the grappling hook runs on other systems, loading them down and making them peripheral victims.

### Replication rate
By instructing the worm to replicate itself regardless of a computer's reported infection status, Morris transformed the worm from a potentially harmless intellectual and computing exercise into a viral denial-of-service attack. Morris's inclusion of the rate of copy within the worm was inspired by Michael Rabin's mantra of randomization.

The resulting level of replication proved excessive, with the worm spreading rapidly, infecting some computers several times. Rabin would eventually comment that Morris "should have tried it on a simulator first".

### Effects
During the Morris appeal process, the US court of appeals estimated the cost of removing the virus from each installation was in the range of $200–$53,000. Possibly based on these numbers, Stoll, a systems administrator known for discovering and subsequently tracking the hacker Markus Hess three years earlier, estimated for the US Government Accountability Office that the total economic impact was between $100,000 and $10,000,000. Stoll helped fight the worm, writing in 1989 that "I surveyed the network, and found that two thousand computers were infected within fifteen hours. These machines were dead in the water—useless until disinfected. And removing the virus often took two days." Stoll commented that the worm showed the danger of monoculture, because "If all the systems on the ARPANET ran Berkeley Unix, the virus would have disabled all fifty thousand of them."

It is usually reported that around 6,000 major UNIX machines were infected by the Morris worm. Graham claimed, "I was there when this statistic was cooked up, and this was the recipe: someone guessed that there were about 60,000 computers attached to the Internet, and that the worm might have infected ten percent of them". Stoll estimated that "only a couple thousand" computers were affected.

The Internet was partitioned for several days, as regional networks disconnected from the NSFNet backbone and from each other to prevent recontamination while cleaning their own networks.

The Morris worm prompted DARPA to fund the establishment of the CERT/CC at Carnegie Mellon University, giving experts a central point for coordinating responses to network emergencies. Gene Spafford also created the Phage mailing list to coordinate a response to the emergency.

Morris was tried and convicted of violating United States Code Title 18 (18 U.S.C. § 1030), the Computer Fraud and Abuse Act, in United States v. Morris. After appeals, he was sentenced to three years' probation, 400 hours of community service, and a fine of US$10,050 (equivalent to $22,000 in 2023) plus the costs of his supervision. The total fine ran to $13,326, which included a $10,000 fine, $50 special assessment, and $3,276 cost of probation oversight.

The Morris worm has sometimes been referred to as the "Great Worm," due to the devastating effect it had on the Internet at that time, both in overall system downtime and in psychological impact on the perception of security and reliability of the Internet. The name was derived from the "Great Worms" of Tolkien: Scatha and Glaurung.

### author
Robert Tappan Morris (born November 8, 1965) is an American computer scientist and entrepreneur. He is best known for creating the Morris worm in 1988, considered the first computer worm on the Internet.