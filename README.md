# cartophrase
Mapping the Earth with words

This project is an open-source proposal to map every location on Earth with a short, memorable sequence of words.

This is a complex socio-technical problem at the intersection of many domains (cartography, human and physical geography, linguistics, culture, mathematics, engineering).

The final output of the project is to be a methodology for:

- Dividing the surface of the Earth into _locations_
- Producing a very large number of _phrases_ composed of short sequences of _words_ for a given language in a way that allows for relatively simple cross-linguistic translation of phrases
- Bijectively _mapping_ the set of phrases to the set of locations

The specifics for the definitions of the italicised words are to be determined as part of the project.

---

Considerations:

- Geographical considerations
  - The movement of land/sea boundaries (tectonic motion, land reclamation)
  - Precision of coordinate and positioning systems, notably due to State restrictions
  - Evolution of population density
- Linguistic-cultural factors
  - The need for clearly distinguishable phrases, both phonetically and orthographically, across complicated linguistic and cultural contexts
    - Meaning of "word"
    - Cross-dialectal phonology
    - Word pronunciation distances will have to be bespoke to each language system
  - Accessibility
- Engineering factors
  - Trade-off between phrase length and wordlist length
    - Fewer words in list -> lower probability of collision
  - Change management
    - Once set, the algorithm _cannot_ change significantly (there can never be a "version 2")
    - Mechanism for notifying affected users of minor changes
  - Collision detection
  - Distribution of phrases -- should phrases be scattered to minimise the probability of proximal confusion (context will typically allow one to distinguish between distant but similar phrases), or should phrases be telescopic to increase memorability (i.e.: I know my neighbourhood starts with A-B-...)?
  - Can we use whole sentences instead of phrases? Likely to be far more memorable, but more complex to generate esp. cross-linguistically.
 
Preliminary work required:

- Generation of a wordlist and systematic phonological apparatus for English
- Exploratory phonological work -- how many distinct words are really totally mutually distinguishable in a given language?
