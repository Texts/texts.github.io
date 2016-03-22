Comments on draft Chapter 2
===========================

 

General Note
------------

A recurring issue with the draft chapters is the lack of a clear structure and
narrative. They read as though your thoughts are not properly organised. As a
result it makes the text difficult to follow and correct. So my key
recommendation is to prepare Chapter structures that include section headings
and sub-headings. Include with this structure some simple notes of what each
section will cover. If you do this before you start writing I am certain you
will find it easier to make progress and the resulting text will be closer to
the final form than at present.

 

e.g.

 

Chapter 2

2.1 Introduction

 

2.2 Definition of $$\Delta$$ values

 

2.3 Requirements of Mass spectrometry

2.3.1 Precision

2.3.2 Sensitivity

2.3.3 Linearity

2.3.4 Scale compression

2.3.5 Contamination

 

2.4 The MIRA mass spectrometer

2.4.1 Description of the instrument

2.4.2 Sensitivity

2.4.4 Linearity

2.4.5 Scale compression

2.4.6 Precision

 

etc…..

 

If you can do this it will also make life easier when reading and commenting on
the chapters. You can work on smaller chunks and give them to me or Alina to
read. We will be able to see where they fit into the narrative.

At present it’s difficult for me to pass back some simple comments without
rewriting extensive sections of the chapter. I’ve rewritten your section on
definition of $$\Delta$$ values below to give you some idea of how you might
approach this chapter. What I have written does not necessarily carry all the
information you might want to put in, nor is it definitive. From the definition
you can clearly identify the key performance requirements for mass spectrometry
in terms of precision, sensitivity etc. This would lead onto a discussion of
MIRA and then on to measurements with MIRA.

 

**Definition of the \\Delta's**

 

This section confuses empirical with various theoretical considerations. This is
largely because I think Huntington et al do so too. In my view it is better to
separate these here and just focus on what we can measure. The theoretical
discussion is best left to the review of the principles of clumped isotope
geochemistry.

 

I would start this section something like this:

 

### 2.2 Practical definition of the $$\Delta$$ value

 

The abundance of a multiply substituted isotopologue of CO$$_{2}$$ is expressed
as an excess $$\Delta$$ value with respect to the theoretical stochastic
abundance (Wang et al., 2004):

 

$$\Delta _{47}} = \left( {\frac{R_{47}}{R_{47}^*} - 1} \right) \times 1000$$

 

$$\Delta _{48}} = \left( {\frac{R_{48}}{R_{48}^*} - 1} \right) \times 1000$$

 

$$\Delta _{49}} = \left( {\frac{R_{49}}{R_{49}^*} - 1} \right) \times 1000$$

 

where $$R_{47-49}$$ represents the measured 47/44, 48/44 and 49/44 ratios
respectively, and $$R_{47-49}^{*}$$ represents the calculated stochastic ratios
for these same species.

For CO$$_{2}$$ we are largely concerned with the isotopologue
$$^{13}$$C$$^{18}$$O$$^{16}$$O (i = 47) but also determine $$\Delta$$ values for
$$^{13}$$C$$^{18}$$O$$^{17}$$O (i = 48) and $$^{13}$$C$$^{18}$$O$$^{18}$$O (i =
49). Note also that given the limited mass resolution of current isotope ratio
mass spectrometers at cardinal masses 47 and 48 there is a contribution to the
measured and calculated ratios of multiply substituted isotopologue species
containing $$^{17}$$O. For example there are three multiply substituted
isotopologue species: $$^{18}$$O$$^{13}$$C$$^{16}$$O,
$$^{18}$$O$$^{12}$$C$$^{17}$$O, and $$^{17}$$O$$^{13}$$C$$^{17}$$O at mass 47.
The contribution of the isobaric $$^{17}$$O containing isotopologues to the
measured  $$\Delta_{47}$$ value is small and thus (Wang et al., 2004):

 

$$\Delta_{^{18}O^{13}C^{16}O}\approx \Delta_{47}$$

 

The ratios $$R_{i}$$ and $$R_{i}^{*}$$ where i = 47-49 are determined from the
measured $$\delta^{i}$$, $$\delta^{13}$$C and $$\delta^{18}$$O values of the
sample CO$$_{2}$$. For $$R^{47}$$:

 

$$R_{47} = \left( {\frac{\delta _{sam - wrg}^{47}}{1000} - 1} \right) \times
R_{47}^{wrg}$$

 

where $$R_{47}^{wrg}$$ is the 47/44 ratio of the working reference gas (wrg) and
is determined as:

 

$$R_{47}^{wrg} = 2 \cdot R_{13}^{wrg} \cdot R_{18}^{wrg} + 2 \cdot R_{18}^{wrg}
\cdot R_{17}^{wrg} + R_{13}^{wrg} \cdot {(R_{17}^{wrg})^2}$$

 

Note that implicit in this treatment is an assumption that the mass spectrometer
working reference gas has a stochastic distribution of isotopes. It is self
evident that this is incorrect since the working reference gas is either at, or
close to equilibrium at the laboratory temperature. However, since the
$$\Delta$$ values are \<1‰ we can make this assumption and carry out a later
linear transformation of the data to take account of the actual reference gas
$$R_{47}$$ value without introducing any significant errors.

The ratios $$R_{13}$$, $$R_{17}$$ and $$R_{18}$$ are determined from the
$$\delta^{13}$$C$$_{VPDB}$$, $$\delta^{17}$$O$$_{VSMOW}$$ and
$$\delta^{18}$$O$$_{VSMOW}$$ values of the working reference gas:

 

$$R_{13} = \left( {\frac{{\delta _{wrg - VPDB}^{13}}}{{1000}} + 1} \right)
\times R_{13}^{VPDB}$$

 

and similar equations for $$R_{17}$$ and $$R_{18}$$. The reference gas ratios
are $$R_{13}^{VPDB}$$ = 0.0112372 (reference), $$R_{17}^{VSMOW}$$ = 0.0004023261
(reference) and $$R_{18}^{VSMOW}$$ = 0.0020052 (reference).

Similarly the $$R_{47}^{*}$$ ratio for a sample corresponding to a stochastic
distribution of the isotopes is given by:

 

$$R_{47}^* = 2 \cdot R_{13}^{sam} \cdot R_{18}^{sam} + 2 \cdot R_{18}^{sam}
\cdot R_{17}^{sam} + R_{13}^{sam} \cdot {\left( {R_{17}^{sam}} \right)^2}$$

 

with $$R_{13}$$, $$R_{17}$$ and $$R_{18}$$ determined using equation 4 and the
measured $$\delta^{13}$$C, $$\delta^{17}$$O and $$\delta^{18}$$O values for the
sample.

 

Substitution of $$R_{47}$$ (equation 2) and $$R_{47}^{*}$$ (equation 5) into
equation 1 allows determination of $$\Delta_{47}$$. Evaluation of
$$\Delta_{48}$$ and $$\Delta_{49}$$ follows the same steps as above.

Examination of equations 1 through 8 shows that measurement of the $$\Delta$$
value of isotopologues in CO$$_{2}$$ requires precise  measurement of the ratios
$$R_{i}$$ ($$i=$$ 45-49) for the sample gas. This can be achieved using
dual-inlet isotope ratio mass spectrometry.

 

### 2.3 Mass spectrometry

 

……etc.

 

 

 
