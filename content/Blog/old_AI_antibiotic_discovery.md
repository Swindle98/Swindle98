+++
title = 'AI antibiotic discovery'
date = 2024-01-26T15:24:44Z
draft = true
+++

Antibiotic discovery could be one of the greatest medical paradoxes of modern times. It is increasingly difficult to discover new antibiotics, with market forces being a major factor slowing development. It takes decades and costs billions to develop new antibiotics, the announcement of a new antibiotic is often accompanied by a drop in stock value, with the developers often <a href="https://www.wired.com/story/the-antibiotics-business-is-broken-but-theres-a-fix/" target="_blank" rel="noreferrer noopener">going out of business</a>. Not the celebratory fanfare you would expect for new products saving humanities future. The more exposure germs get to the antibiotics the more likely they are to acquire resistance to the antibiotic. This leads health officials to hold back the use of new antibiotics for the worst of cases, where current antibiotics are no longer effective. Spending all this money to let it sit on a shelf for years, isn’t the most attractive opportunity for investors. Drug companies could have spent their money developing a new treatment for diabetes, the patients are often wealthy and it’s a chronic illness so the company gets a large stable income for decades. Compare that to antibiotics which are often required in undeveloped nations, and treatment may only be for a couple of weeks, producing only small amounts of random income. It starts to become rather clear why investors aren’t interested in antibiotics.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><br>Another factor at play once funding has been attained is the difficulty of discovering the new antibiotics; we’ve found all the low hanging fruit. The screening methods of the last century of just taking soil samples and looking for antibiotics is now just presenting compounds we already know and use. The latter half of the 20th century saw scientists trying to synthesise their own chemicals,<a rel="noreferrer noopener" href="https://longitudeprize.org/blog-post/serious-lack-new-antibiotics-pipeline-says-who" target="_blank"> but with little success</a> . Current methods have resulted in screening chemical libraries containing thousands to millions of chemicals, a costly and time expensive experience. This is where the Colin lab’s work comes into play. In their recent paper “<a rel="noreferrer noopener" href="https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1#" target="_blank">A deep learning approach to antibiotic discovery”</a> they document how they’ve used machine learning, to predict which compounds in a vast library might have antibiotic abilities, allowing them to discover a new antibiotic that acts in a way that has previously been undocumented.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><br><strong><em>Building their algorithm</em></strong><br>The embedded video by 3brown1blue goes into the basics of neural networks, but simply put; in a normal program you give it rules, and input data and it comes back with an answer. For a neural network, you provide it with the input data, and it creates its own rules, that can be used to answer the given question again in the future. Neural nets must be trained first (this is actually what you're doing when google asks you to prove you’re human “please select the…”), here they took a small subset of the catalogue of drug they wanted to investigate, they tested them for their antibiotic tendencies against <em>E. coli</em> in the lab first. Then they told the neural net the results, the rules the neural net created while it was trained, were then applied to the rest of the dataset (a catalogue of drugs previously trialled against tuberculosis) to predict their antibiotic abilities.</p>
<!-- /wp:paragraph -->

<!-- wp:embed {"url":"https://www.youtube.com/watch?v=aircAruvnKk","type":"video","providerNameSlug":"youtube","responsive":true,"className":"wp-embed-aspect-16-9 wp-has-aspect-ratio"} -->
<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">
https://www.youtube.com/watch?v=aircAruvnKk
</div></figure>
<!-- /wp:embed -->

<!-- wp:paragraph -->
<p><br>A major difference between this experiment and previous studies is that previously, characteristic features of the chemicals were fed in by hand (or a program trained to recognise in the same way), this is called supervised learning. This algorithm also reads the pure chemical data (information about all the bonds and atoms, not limited by what a human thinks is important) and is allowed to make its own rules, this is unsupervised learning. The combination of the two allow the algorithm to generalise enough in order to pick drugs that a scientist wouldn’t notice, but the inclusion of the characteristic feature data, prevents it from overgeneralising and being too far off from potential drugs.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":63,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://windlemeuk.files.wordpress.com/2020/04/1artboard-1net-input.jpg?w=1024" alt="" class="wp-image-63"/><figcaption class="wp-element-caption">Both supervised and unsupervised approaches were used in order to predict antibioitic ability of the drugs against <em>E.Coli</em></figcaption></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>The chemicals from the wider dataset predicted to have antibiotic properties were then scored by their similarities to known antibiotics, the highest predicted and most different chemicals were then tested. Of the chemical tested a large percentage had no effect, but the experiments did reveal a number of chemicals that were effective and previously undiscovered.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><br>The scientists were particularly excited by the discovery of the compound they coined halicin, an antibiotic that they found effective against a wide variety of bacteria including those such as <em>A. baumannii</em> and <em>C.difficille</em> pathogens that WHO classify as highest threats for multidrug antibiotic resistance . When they tried to work out the mechanism of action for halicin, they first tried to produce a halicin resistant strain, by sequencing the resistant strain they could compare that to the non-resistant strain, and the changes could show how the cell has overcome the drug, suggesting how the drug was affecting the cell in the first place. However, they were unable to produce a halicin resistant strain. Instead the scientists characterised the compound by seeing how the bacteria reacted in sub lethal concentrations. They found that halicin prevented a hydrogen ion gradient essential for energy production in the cell, the same gradient that allows mitochondria to produce their energy in our cells (proton motive force). Animal models showed that the compound could be systematically applied, and cleared up <em>A.baumannii</em> infections, without being toxic to the mouse.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><br>This application of machine learning in drug discovery has a real potential to reduce costs, and time during the initial discovery phase. However, throughout the paper the authors continually remind the reader that the neural network on its own isn’t enough, and that scientists need to submit the predicted drugs to further experiments in order to confirm the antibiotic properties. The algorithm is another form of intuition before the experiments can begin. Of course, a large number of candidate chemicals are useless if the wider pharmaceutical industry is lacking the motivation to develop them into dugs… for that we need directional and forward thinking government policy…. Oh.