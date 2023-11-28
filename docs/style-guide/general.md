# General Guidelines 

Follow these guidelines when writing any documentation-related text: 

## The four C’s 

Make sure your documentation complies with the following requirements: 

- **Clear**: Write with your target audience in mind, but keep it approachable by avoiding idioms, uncommon terms, and complicated sentences. 

    ??? tip "Do’s and Don'ts"

        Here you can find some scenarios to better illustrate clarity: 

        - **Do** use the present tense to describe the system operation. 
        - **Do** use affirmative sentences to indicate the correct operation whenever possible. 
        - **Do** use common and consistent terms across the documentation. For example, use the word *amount* when referring to monetary values instead of using *value*, *sum*, and other terms interchangeably. 
        - **Do** use the active voice whenever possible. Passive voice sentences usually omit the agent (the party that performs the action) and are sometimes longer or harder to understand that active voice sentences. 
        - **Don’t** use idioms that might confuse unfamiliar readers. For example, don’t rewrite this guideline as *Idioms can be a red herring*. 

- **Complete**: Write all the information that the reader needs. Include links to relevant sources when necessary and avoid using ellipsis ``...`` or the word ``etc``. 

    ??? tip "Do’s and Don'ts"

        Here you can find some scenarios to better illustrate completeness:

        - **Do** include all supported inputs for a field or a rule to unequivocally identify them. For example: *"Allowed countries are: ``CA``, ``US``, and ``FR``."* if only those are allowed; or *"Input a [ISO 3166 Alpha-2](https://www.iban.com/country-codes) country code."* If all country codes are allowed.
        - **Do** mention common errors that users encounter and a way to avoid them.
        - **Do** mention the output of the operations that you describe in your how-to guides. That way the reader knows what to expect at the end.
        - **Don’t** leave important information for the reader to imply. For example, don’t use incomplete lists like *"(JAN, FEB, MAR, etc.)"*  

- **Concise**: Write only the information that will generate value to the reader. Strive to provide your readers with the information that they need to perform their role. 

    ??? tip "Do’s and Don'ts"

        Here you can find some scenarios to better illustrate conciseness:
        
        - **Do** start your descriptions with a noun instead of repeating the term or starting with ``It is`` or `This item`. For example: *"**Weight**: Number from 0 to 1 that indicates the percentual impact of the concept on the final sum. Where 0 is 0% and 1 is 100%"*.
        - **Don’t** include information that is irrelevant to the reader. For example, you can rewrite the sentence *"When you click the Search button, the system performs an SQL query on three different tables from the database to find items that match your search criteria.”* as *“Click Search to find items that match your search criteria.”* 

- **Correct**: Write information that know is accurate. Always review the information with an SME (Subject Matter Expert) and never include assumptions. 

    ??? tip "Do’s and Don'ts"

        Here you can find some scenarios to better illustrate correctness:
        
        - **Do** take notes of your meetings with SMEs to make sure that the information you include is accurate.
        - **Do** check that you understand correctly new terms with the SMEs with questions like *“So the system only saves changes once the user clicks **Save**, right?”*.
        - **Don’t** write any information that you’re not completely certain.
        - **Don’t** be afraid of asking questions.

## Know your audience

Make sure you know who your documentation’s target audience is. Technical readers are interested in the specifics of the system’s operation while non-technical readers usually want to understand what the system can do and whether it fits their needs. You can use diagrams accordingly. For example, class diagrams tell technical readers how the system treats information on a specific level.

```kroki-plantuml
@from_file:assets/class_diagram.puml
```

### Documentation Tone

Many documentation sites use the [Diátaxis](https://diataxis.fr/) framework that categorizes documents into:

- **Explanation**: Understanding-oriented document that introduces a concept to readers.
- **How-to Guides**: Task-oriented document that describes a process to readers step by step.
- **Reference**: Information-oriented document that specifies the details of a system to readers.
- **Tutorial**: Learning-oriented document that introduces readers to one or more concepts while they follow a series of steps.

Explanation documents give the most freedom regarding the tone that you can adopt to introduce readers to new concepts. Use examples whenever possible and avoid using a condescending tone.

Reference documents are mostly impersonal, as they simply contain details of the system and are a series of informative statements in present tense.

Tutorials and how-to guides must use imperative sentences and avoid using *please*. This might sound as unpolite, but it is necessary to assert the authority of the documentation. These documents indicate the steps to achieve a correct operation of the system. Following them is mandatory.
