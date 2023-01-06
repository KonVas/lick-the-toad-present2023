
# Table of Contents

-   [Introduction](#org8341dd0)
-   [Lick the Toad](#orgc9e0530)
-   [Bridging the audience agency in musical interaction](#org47c18d8)
-   [Background](#org0838433)
-   [Ltt: machine Learning in the browser](#orgd83d99a)
-   [Ltt&rsquo;s creative directions](#orgea06e34)
-   [Discussion](#orgbb203ee)
-   [Thanks](#orgc79a053)




<a id="org8341dd0"></a>

# Introduction


<a id="orgc9e0530"></a>

# Lick the Toad

Ltt is a web interface designed for bridging the gap between performer(s) and audience, allowing former and latter to engage interactively.


<a id="org47c18d8"></a>

# Bridging the audience agency in musical interaction

It allows for real time of data interaction between clients and server offering an ideal tool to share data for musical interpretation on the fly.


## Back to the parlour

> &#x2026; as the schism between ‘popular’ and ‘art’ deepened, and
> the latter demanded increasing levels of virtuosity in order
> to realise musical ideas, performance of certain strands of
> contemporary music became nearly impossible for anyone
> but professionals; disappearing from the ‘soiree’ repertoire.

*Fischman, R. (2011). Back to the parlour. Sonic Ideas – Ideas Sónicas, 3(2): 53–66.*


## Some implementation notes:

1.  Real time communication using web sockets<sup><a id="fnr.1" class="footref" href="#fn.1" role="doc-backlink">1</a></sup>
2.  Sonifications on users&rsquo; devices.
3.  OSC communication with: MaxMSP, SuperCollider, Pure Data, etc.


<a id="org0838433"></a>

# Background

![img](https://upload.wikimedia.org/wikipedia/commons/0/00/Telharmonium_-_Scientific_American_1907_%28zoomed_400%25%2C_brightened%29.jpg)


## Looking Back

“The Art of and Apparatus for Generating and Distributing Music Electrically”.<sup><a id="fnr.2" class="footref" href="#fn.2" role="doc-backlink">2</a></sup> [1](#org145842f)

<table id="org145842f" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Name</th>
<th scope="col" class="org-left">Instrument</th>
<th scope="col" class="org-right">Year</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">Puskás</td>
<td class="org-left">Telefonhírmondó</td>
<td class="org-right">1893</td>
</tr>


<tr>
<td class="org-left">Cahill</td>
<td class="org-left">Telharmonium</td>
<td class="org-right">1895/97</td>
</tr>


<tr>
<td class="org-left">Gray</td>
<td class="org-left">Musical Telegraph</td>
<td class="org-right">1874</td>
</tr>


<tr>
<td class="org-left">Ader</td>
<td class="org-left">Théâtrophone</td>
<td class="org-right">1881</td>
</tr>


<tr>
<td class="org-left">Soemering</td>
<td class="org-left">n/a</td>
<td class="org-right">1809</td>
</tr>
</tbody>
</table>

*Crab, S. (2013). The ‘Telharmonium’ or ‘Dynamophone’ Thaddeus Cahill, USA 1897.*

<div class="NOTES" id="org5bb199e">
<p>
In 1895 Thaddeus Cahill submitted his first patent for the Telharmonium
By Unknown author - The World&rsquo;s Work, June 1906, vol. XII, no. II, Public Domain, <a href="https://commons.wikimedia.org/w/index.php?curid=112285881">https://commons.wikimedia.org/w/index.php?curid=112285881</a>
</p>

</div>


## Looking Forward

Modern takes using telecom: the networked music paradigm *Collins, N., & Escrivan Rincón, J. d. (2011). The Cambridge companion to electronic music. Cambridge: Cambridge University Press.*

Previous works by the author in this field:

-   [BEER Pea Stew: Recalibrated](https://serkansevilgen.com/docs/01_ICLC_2021_Sevilgen_Vasilakos_Wilson.pdf) (Wilson, Vasilakos, Lorway, Margetson, Yeung).
-   [ICE: Symphony in Blue 2.0](https://serkansevilgen.com/docs/01_ICLC_2021_Sevilgen_Vasilakos_Wilson.pdf) **based on Kamran Ince&rsquo;s initial work** (Vasilakos, Sevilgen, Dagdeviren, Wilson)


<a id="orgd83d99a"></a>

# Ltt: machine Learning in the browser


## Client Collection Data

A client allows to train a model in a web browser and triger predictions based on a regression algorithm. Once the training process is done the system offers visualization of the output values. The sound generation is based on a Markov chain module which is generating predictions based on the ml predictions. At the same time the client is able to send these data to other clients &ldquo;listening&rdquo;  for incoming OSC messages.


## Notes on ML in Computer Music and Digital Arts

For some machine learning in Electronic Music literature as follows:

-   Vasilakos, K. (2022). A Networked Hybrid Interface for Audience Sonification and Machine Learning. Revista Vórtex, 10(1) <http://dx.doi.org/10.33871/23179937.2022.10.1.4695>
-   Collins, N. (2015). Live Coding and Machine Listening. In Proceedings of the First International Conference on Live Coding (pp. 8). Leeds, UK.
-   Fiebrink, R., & Sonami, L. (2020). Reflections on Eight Years of Instrument Creation with Machine Learning. In R. Michon, & F. Schroeder, Proceedings of the International Conference on New Interfaces for Musical Expression (pp. 282–288). Birmingham, UK: Birmingham City University.
-   Baalman, M. (2020). The machine is learning.
-   Amershi, S., Cakmak, M., Knox, W. B., & Kulesza, T. (2014). Power to the People: The Role of Humans in Interactive Machine Learning. AI Magazine, 35(4), 105–120. <http://dx.doi.org/10.1609/aimag.v35i4.2513>


<a id="orgea06e34"></a>

# Ltt&rsquo;s creative directions

<div class="NOTES" id="org370f070">
<p>
Ltt has been used as a standalone app for collective sonifications of bystanders and remote participants but since then it has taken many spins including a real time chat engine amongst peers.
</p>

</div>


## Live Coding: what now?

In live coding performances, there is always the question of how a coder is taking their decisions while changing the code on the fly, described also as &ldquo;kairotic coding&rdquo;. *Cocker, E. (2018). What now, what next — kairotic coding and the unfolding future seized. Digital Creativity, 29(1), 82–95. <http://dx.doi.org/10.1080/14626268.2017.1419978>*


### Ongoing Work

A study on live coding using ltt and stochastic processes<sup><a id="fnr.3" class="footref" href="#fn.3" role="doc-backlink">3</a></sup> in SuperCollider&rsquo;s JITLib.

    {
    	[nil].choose;
    }

[[nil]​](https://youtube.com/watch?v=IrGk0yrfbOY)


<a id="orgbb203ee"></a>

# Discussion

While ltt serves both as a standalone and live coding tool, it arguably allows for a greater coherence amongst peers on live performance. Similar to the concept of &ldquo;back to the parlour&rdquo; where members of the audience are able to enact an impromptu improvisation.


<a id="orgc79a053"></a>

# Thanks

Courtesy to the majestic Org mode

![img](https://upload.wikimedia.org/wikipedia/commons/a/a6/Org-mode-unicorn.svg)

&#x2026;and the powerful SuperCollider

![img](https://upload.wikimedia.org/wikipedia/commons/6/60/SuperCollider_logo.svg)


# Footnotes

<sup><a id="fn.1" href="#fnr.1">1</a></sup> Web sockets is a real time communication mechanism that allow web pages to send and receive data amongst peers.

<a id="org3458b00"></a>

<a id="org48f5c2f"></a>
<~/Documents/bibliography.bib>

<sup><a id="fn.2" href="#fnr.2">2</a></sup> A [new field of electronic musical instruments](https://120years.net/wordpress/the-telharmonium-thaddeus-cahill-usa-1897/) and [electronic musical instruments creation using telegraphy](https://artsandculture.google.com/story/iAWRKDY1jD1jKA).

<sup><a id="fn.3" href="#fnr.3">3</a></sup> Stochastic synthesis is coined by Iannis Xenakis, with some of the most famous works Legend Air and Gendy system.
