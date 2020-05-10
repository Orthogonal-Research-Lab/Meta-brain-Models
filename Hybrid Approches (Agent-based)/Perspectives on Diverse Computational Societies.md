## Perspectives (on and for) Diverse Computational Societies  

How do we represent the potential social structures generated by the biological underpinnings of cognition? We propose an emerging approach that includes computational agents situated in an environmental context of various geometric perspectives. These perspectives are analyzed and synthesized by the agent’s biology. Stimulus diversity is achieved introducing stimuli from various perspectives. This biology is represented by a hybrid connectionist/genotype-to-phenotype mapping, and results in an internal model (phenotype). An internal model not only interacts with the internal models of other agents, but can also synthesize different sources of information embodied in environmental stimuli. These interactions between internal models are the source of diverse computational societies, which can be monitored in real-time using various measures of diversity or subjected to network analysis.

#### Introducing Environmental Relativism
Assume a network of different perspectives on a common type of stimuli. Agents take a subset of these perspectives, a network model of shared cultural context. We can use various transformations of images or geometric shapes as perspective data. These stimuli can exist as affine transformational perspectives in a real world context, or deformed transformational perspectives in a virtual world context. Affine perspectives (see Part A, graphical abstract) are those where the shape is shifted in a way that preserves the ratio between shape components. For example, for a series of points and lines, the resulting shape preserves the original relational information. By contrast, deformed perspectives (see Part B, graphical abstract) are a distortion of the original image where the ratio between shape components is modified. For a series of points and lines, this could be represented by using parametric curves rather than straight lines. Population of agents with different perceptual histories but same innate traits results in overlapping populations of perspectives.

Training agents on multiple perspectives has numerous advantages when understood as viewpoints. In a classic paper, Rouse (1999) discusses the role of first- and third-person views in video gaming, particularly the importance of seeing objects and worlds from various perspectives. Incorporating different views of the same set of objects contributes to improved performance and social presence (Gorisse et.al, 2017; Galvan Debarba et.al, 2017). The perspectives require the rotation of angles, alignments, and paths of motion, and a diversity of these viewpoints have a significant impact on the cognitive states of the viewers (Misslivirose, 2017). We predict that these findings on viewpoints  will also hold true for computational agents. For example, Ye et.al (2020) used relativistic perspectives are used to introduce agents to a diverse set of inputs in an open-ended manner, with which  they were able to generalize a deep learning model for one-shot learning. Additionally, the degrees of freedom introduced by transformations of image perspective contributes to the need for greater social presence. Demaine et.al (2016) help us understand this in terms of computational complexity, which has been further demonstrated in world design of video games such as Pac-Man (Viglietta, 2013), Minesweeper (Kaye, 2000), and classic Nintendo games (Aloupis et.al, 2014).

We further predict that some agents will develop a preference for some perspectives over others, which can evolve on the basis of a generative internal model. This is based on a hybrid connectionist/popgen/GA model first described in Alicea (2007). While conventional connectionist models focus on pattern recognition and associative learning, our hybrid connectionist model takes a different approach. Our approach is to incorporate a genetic representation to produce an internal model that represents a simple behavioral phenotype. In this way, we can produce stereotypical behaviors that incorporate environmental feedback. Yet more importantly, we can also produce phenotypic diversity across agents, which provides quite a different perspective on the study of behavior.

#### Hybrid Connectionist Approach to Biorealism
We use a biologically plausible approach that approximates the relationship between genotype (G) and phenotype (P). Rather than the brain, we take inspiration from population genetics to represent the contributions of information encoded in genes (g), the temporal expression of these genes (t), environmental influences (e), and stochastic contributions (s) to represent a behavioral phenotype. 

Our basic genetic representation is a bipartite graph that estimates the genotype to phenotype relationship, or G → P. We call this the _simple epistatic model_ (see Part C, graphical abstract). The interaction matrix WGP represents a non-reversible mapping. These elements can be weighted by parameters e and s to account for uniform influences of environment and stochastic effects. Both of these parameters are summary representations of feedback from the environment (see Figure 1). When values for e and s approach 1.0, the G → P relation can partially recover the inverse mapping P → G. 

Our more complex representation involves the use of deep connectionist models (graphs with many layers), and  We refer to this as the _complex epistatic model_ (see Part D, graphical abstract), and can be compared performance-wise to the simple model. As this model has many layers, recovering the inverse mapping (P → G) is impossible. However, the representation of parameters e and s are more details, and consist of a heterogeneous set of units (a distinct layer) in the model (see Part C, graphical abstract) .

Rather than using a black box nervous system which processes environmental information, we use a genetic representation which uses the contributions of endogenous genetic contributions with environmental input and feedback to process information and produce a phenotype (see Part E, graphical abstract). Both the simple and complex epistatic models represent an internal model, which is unique to each agent in the population. This allows us to emphasize the uniqueness of individuals in a population. This is particularly true for the complex model, which can be enabled by even a small population of clones with the same initial genotype. 

#### Interactions Between Internal Models
This internal model is an approximation of the multitude effects that arise from genetics, physiology, and environment. Across a population of agents, we can now examine the interactions between agents and among various stimuli. These interactions constitute the environment in which the internal models operate. This allows us to approximate a number of effects, including: preference-based selection, which suppresses similar but less-preferred stimuli, perceptual biases such as an aversion to selected stimulus features and non-realistic object physics, and the attraction-repulsion behavior of other agents.

While our internal model can potentially represent great population-level diversity, we also need a method to measure this diversity in a way that translates to the study of behavior. Measures of diversity include applications of mutual information, or a more contextual description based on soft (fuzzy) classification to deal with vagueness and composition (Barbosa, 2015). These measures of diversity provide a statistical summary of the phenotype, the output of which (as in Part E of the graphical abstract) can either be numeric or mapped to a bodily representation.

Our last prediction is that the phenomenon of cumulative culture (Mesoudi & Thornton, 2018; Sasaki & Biro, 2017) can also serve as a guide to explaining behaviors exhibited by our agents. In a typical collective behavior model, there is some form of communication between the agents as they align  their behavior. While coordination (and in turn communication) is non-existent among our agents, cumulative behavior nevertheless provides a means for convergent behavior.

### Graphical Abstract
<p align="center">
  <img width="417" height="449" src="https://github.com/Orthogonal-Research-Lab/Proposals/blob/master/Collective%20Intelligence%202020/graphical-abstract.png"><BR>
 Parts A and B are the perspectives presented to the agent, parts C and D are the architectures, and part E is an example of the phenotypic mapping. Click to enlarge.
</p>

### References
Alicea, B. (2007). Towards a theory of human intraspecific variation for ergonomics and human modeling. _Society for Automotive Engineering (SAE) Digital Human Modeling_, #2007-01-2461.

Aloupis, G., Demaine, E.D., Guo, A., and Viglietta, G. (2014). Classic Nintendo games are (NP-) hard. _arXiv_, 1203.1895.

Barbosa, A.M. (2015). fuzzySim: applying fuzzy logic to binary similarity indices in ecology. _Methods in Ecology and Evolution_, 6, 853-858.

Demaine, E.D., Lockhart, J., and Lynch, J. (2016). The Computational Complexity of Portal and Other 3D Video Games. _arXiv_, 1611.10319.

Galvan Debarba, H., Bovet, S., Salomon, R., Blanke, O., Herbelin, B., and Boulic, R. (2017). Characterizing first and third person viewpoints and their alternation for embodied interaction in virtual reality. _PLoS One_, 12(12), e0190109. doi:10.1371/journal.pone.0190109.

Gorisse, G., Christmann, O., Amato, E.A. and Richir, S. (2017). First- and Third-Person Perspectives in Immersive Virtual Environments: presence and performance analysis of embodied users. _Frontiers in Robotics and AI_, 4, 33. doi:10.3389/frobt.2017.00033.  

Kaye, R. (2000). Minesweeper is NP-complete. _The Mathematical Intelligencer_, 22(2), 9–15.

Mesoudi, A. & Thornton, A. (2018). What is cumulative cultural evolution? Proceedings of the Royal Society of London B, 285(1880), 20180712. http://doi.org/10.1098/rspb.2018.0712.

Misslivirose (2017). Exploring the Idea of Dynamic Perspectives in Virtual Reality. _Liv Ericson Medium_, January 12. https://livierickson.com/blog/exploring-the-idea-of-dynamic- perspectives-in-virtual-reality/

Rouse, R. (1999). What's Your Perspective? _Computer Graphics_, 33(3). doi:10.1145/330572.330575.

Sasaki, T. & Biro, D. (2017). Cumulative culture can emerge from collective intelligence in animal groups. _Nature Communications_, 8, 15049. doi:10.1038/ncomms15049.

Viglietta, G. (2013). Gaming Is A Hard Job, But Someone Has To Do It! _arXiv_, 1201.4995.
 
Ye, C., Khalifa, A., Bontrager, P., and Togelius, J. (2020). Rotation, Translation, and Cropping for Zero-Shot Generaliztion. _arXiv_, 2001.09908.