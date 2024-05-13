
![[Pasted image 20240513204021.png]]

## Phase 2 - System Level Design
- During phase 2, the development of the architecture of the product continues from phase 1 - concept development
- i.e., the product specifications identified in the Contract Book continue to become more defined
- Phase 2 includes the definition of the product architecture and the decomposition into functional & physical elements
![[Pasted image 20240513204120.png]]

- This definition and decomposition can be clearer for physical products, but still relevant for software, etc.
- Think about the use of classes, subsystems, and interfaces in Java program development, for example.

## Product Architecture
- Product Architecture can be described as:
  - "The scheme by which the functional elements of the product are arranged into physical chunks"
- Architectural decisions allow the detailed design and testing of these physical blocks to be assigned to teams, individuals, and/or suppliers, so that the development of different portions can be carried out simultaneously
![[Pasted image 20240513204245.png]]

- Products can be thought of both in functional and physical terms:
  - Functional – individual operations and transformations that contribute to its overall performance
    - e.g., for a printer – "communicate with host computer"
  - Physical – parts, components, and subassemblies that implement the product’s functions

- The physical elements of a product are typically organized into several major building blocks – called chunks
- These chunks become the building blocks for the product or family of products

- Each chunk is then made up of a collection of components which implement the functions of the product.

![[Pasted image 20240513204539.png]]

### Phase 2 – System-level design
- The architecture of a product is therefore the scheme by which the functional elements of the product are:
  - Arranged into physical chunks
  - By which the chunks interact

#### Modular or integral architecture
- A key characteristic of product architecture is the degree to which it is either:
  - Modular, in which:
    - Each chunk implements one or a few functions entirely.
    - The interactions between chunks are well defined.
  - Modular architecture has advantages in simplicity and reusability for a product family or platform.

#### Integral
- Functional elements are implemented by multiple chunks, or a chunk may implement many functions.
- The interactions between chunks are poorly defined.
- Integral architecture generally increases performance and reduces costs for any specific product model.

e.g.

![[Pasted image 20240513204744.png]]
![[Pasted image 20240513204805.png]]

### Concepts and levels
- The concepts of integral and modular apply at several levels:
  - System
  - Sub-system
  - Component
![[Pasted image 20240513204856.png]]

- Product Architecture is decomposition + interactions
  - Decomposition
  - Interactions
    - Within chunks
    - Across chunks

- There are three main types of modular architecture:
  1. Slot-modular (the most common type)
    - Each of the interfaces between chunks in a slot-modular architecture is of a different type from the others – therefore, the various chunks in the product cannot be interchanged

![[Pasted image 20240513204944.png]]

- There are three types of modular architecture:
  2. Bus-modular
    - There is a common bus to which the other chunks connect via the same type of interface

![[Pasted image 20240513205012.png]]


- There are three types of modular architecture:
  3. Sectional-modular
    - All interfaces are of the same type, there is no single element to which all the other chunks attach.
    - The assembly is built up by connecting the chunks to each other via identical interfaces.

![[Pasted image 20240513205049.png]]

### Implications of product architecture

- There are implications to the decisions you make about product architecture.
- Product change
  - Modular chunks allow changes to be made to a few isolated functional elements of the product without necessarily affecting the design of other chunks.
- Motives for change include upgrades, add-ons, adaptation, wear, consumption, flexibility in use, reuse.

- Product variety
  - Variety refers to the range of product models the firm can produce within a particular time period in response to market demand.
  - Products built around modular product architectures can be more easily varied without adding tremendous complexity to the manufacturing system.
  - e.g., mobile phone handset design, portable audio

### Planning a modular product line: Commonality Table
![[Pasted image 20240513205220.png]]

### Implications of product architecture
- Component standardization
  - The use of the same component or chunk in multiple products.
  - If a chunk implements only one or a few widely useful functional elements, then the chunk can be standardized and used in several different products.
  - Example – standard batteries
- Product performance
  - How well a product implements its intended functions.
  - Product performance characteristics include speed, efficiency, life, accuracy, and noise.
- Manufacturability
  - The product architecture also directly affects the ability of the team to design each chunk to be produced at low cost.
  - Product development management
  - Responsibility for the detail design of each chunk is usually assigned to a relatively small group within the firm or to an outside supplier.
  - Chunks are assigned to a single individual or group because their design requires careful resolution of interactions among components within the chunk.

### Recap: fundamental decisions to make at Phase 2
- Integral vs. modular architecture?
- What type of modularity?
- How to assign functions to chunks?
- How to assign chunks to teams?
- Which chunks to outsource?


## Phase 3: Detail Design
![[Pasted image 20240513205536.png]]
- We need to emphasise manufacturing issues throughout the process
- If we don’t we may not be able to make our product!
- The need to think about this becomes very important at the ‘detail design’ stage


- Phase 3 includes
    - The complete specification of the
        - geometry (i.e. physical dimensions)
        - materials, and
        - tolerances
      of all the unique parts in the product, and
    - The identification of all of the standard parts to be purchased from suppliers
- Two critical issues addressed in the detail design phase are
    - Production cost
    - Robust design (or performance)

### Control documentation
- The output of Phase 3 is the control documentation for the product
- The control documentation is:
    - The drawings or computer files describing the geometry of each part to be made and its production tooling
    - The process descriptions for the fabrication and assembly of the product
    - The specifications of the parts to be purchased

### Design for X Topics
- Design for Manufacturing
- Design for Production
- Design for Assembly
- Design for Recycling/Disposal
- Design for Life Cycle
- Design for Environment

### Design for Manufacturing (DFM)
- DFM is a design strategy that requires
    - The expertise of multiple team members
    - The use of basic design rules, guidelines, and cost models

- DFM often results in
    - Significant cost reduction
    - Improvement in product quality
    - The development of cross-functional expertise within the organization

#### Focus on manufacturability
- Focusing on how a product can be manufactured helps the design team to find solutions to these design issues:
    - Detailed design decisions can have substantial impact on product quality and cost
    - Development teams face multiple, and often conflicting, goals

- It is important to have metrics with which to compare alternative designs
- Dramatic improvements often require substantial creative efforts early in the process
- A well-defined method helps the decision-making process


#### Manufacturing Cost
- Manufacturing cost has a major effect on the economic success of a product
- An organization wants to ensure it obtains the highest profit margin possible and therefore tries to identify the lowest manufacturing cost
- Economically successful design is about ensuring high product quality

- Design for manufacturing (DFM) is one way of achieving this goal
- Effective DFM practice leads to low manufacturing costs without sacrificing product quality
- DFM is only effective if the cross-functional team is effective


#### Design for Manufacturing (DFM) and the phases
- DFM begins during phase 1 - concept development - when the products’ functions and specifications are being determined
- When choosing a product concept, cost is almost always one of the criteria on which the decision is made

![[Pasted image 20240513225758.png]]

- During phase 2 – system-level design - the team makes decisions about how to break up the product into individual components
- These decisions are largely based on the expected cost and manufacturing complexity implications

![[Pasted image 20240513225824.png]]

- Accurate cost estimates become available during phase 3 – detail design
- At this point, many more decisions are driven by consideration of how the product will be manufactured

### Phase 4 Testing and Refinement
- The testing & refinement phase involves the construction and evaluation of multiple production versions of the product

- Prototype definitions
- Uses of prototypes
- Types of prototypes
- Planning a prototype
- Prototyping strategy

• Prototyping is done throughout the development process 
• It becomes most important at the testing stage

![[Pasted image 20240513230154.png]]

Prototyping is the process of quickly putting together a working model (a prototype) in order to test various aspects of a design, illustrate ideas or features and gather early user feedback.- Wikipedia

IEEE defines prototyping as “ A type of development in which emphasis is placed on developing prototypes early in the development process to permit early feedback and analysis in support of the development process.

### What is a Prototype?
- A prototype is
    - “an approximation of the product along one or more dimensions of interest”
    - Industrial designers produce prototypes of their concepts, such as models
    - Engineers prototype a design
    - Software developers write prototype programs
    - Prototyping is the process of developing such an approximation of the product

- There are 3 phases of prototyping
    - Alpha prototypes
        - Are typically used to assess whether the product works as intended
    - Beta prototypes
        - Are typically used to assess reliability and to identify remaining bugs in the product
    - Pre-production prototypes
        - Are the first products produced by the entire production process

#### Alpha
- There are 3 phases of prototyping
    - Alpha prototypes
        - Are typically used to assess whether the product works as intended
    - Beta prototypes
        - Are typically used to assess reliability and to identify remaining bugs in the product
    - Pre-production prototypes
        - Are the first products produced by the entire production process

#### Beta
- Later (beta) prototypes are usually built with parts supplied by the intended production processes
- But may not be assembled using the intended final assembly process
- Beta prototypes are extensively evaluated internally and are also typically tested by customers in their own use environment
- The goal for the beta prototypes is usually to answer questions about performance and reliability in order to identify necessary engineering changes for the final product


#### Uses of Prototypes
- There are four main uses of prototypes:
    1. Learning
        - Answering questions about performance or feasibility, such as
            - “Will it work?”
            - “How well does it meet the customer needs?”
        - For example, a proof-of-concept model
    2. Communication
	    - Demonstration of a product to get feedback from all stakeholders
	        - e.g. top management, vendors, partners, extended team members, customers and investors
	    - A physical, tactile, 3D representation of a product is much easier to understand than a verbal description or even a sketch of a product
	        - e.g. 3D physical models of style or function
	3. Integration
	    - Prototypes are used to ensure that components and subsystems of the product work together as expected
	    - Comprehensive physical prototypes are the most effective as integration tools in product development projects because they require the assembly and physical interconnection of all of the parts and subassemblies that make up a product
	    - The integration of the prototype forces coordination between different members of the product development team
	    - For example: alpha or beta test models
	4. Milestones  Provide goals for the development team’s schedule Milestone prototypes are defined in the product development project plan  ‘Go/no go’ decisions can be at these points

- The number of such prototypes and their timing is one of the key elements of the overall development plan
- As a base case, the development team should consider using alpha, beta, and pre-production prototypes as milestones
    - e.g. first testable hardware


#### Types of Prototype
- Prototypes can be classified along two dimensions
    - Physical v analytical
        - Physical – e.g. a wooden model
        - Analytical – e.g. a computer model
    - Comprehensive v focussed
        - Comprehensive - most of the attributes of the real product
        - Focused – one or a few attributes of the real product

#### Physical
- Physical prototypes are tangible artefacts created to approximate the product
- Aspects of the product of interest to the development team are actually built into an artefact for testing and experimentation
- Examples of physical prototypes include
    - Models which look and feel like the product
    - Proof-of-concept prototypes used to test an idea quickly
    - Experimental hardware used to validate the functionality of a product

#### Analytical
- Analytical prototypes represent the product in a non-tangible, usually mathematical, manner
- Interesting aspects of the product are analysed, rather than built
- Examples of analytical prototypes include
    - Computer simulations
    - Systems of equations encoded within a spreadsheet
    - Computer models of three-dimensional geometry

#### Comprehensive
- Comprehensive prototypes implement most, if not all, of the attributes of a product
- A comprehensive prototype corresponds closely to the everyday use of the work prototype – i.e. it is a full-scale, fully operational version of the product
- An example of a comprehensive prototype is one given to customers in order to identify any remaining design flaws before committing to production

#### Focused
- Focused prototypes implement one, or a few, of the attributes of a product
- Examples of focused prototypes include foam models to explore the form of a product and wire wrapped circuit boards to investigate the electronic performance of product design
- A common practice is to use two or more focused prototypes together to investigate the overall performance of a product
- One of these prototypes is often a “looks-like” prototype, the other a “works-like” prototype
- By building two separate focused prototypes, the team may be able to answer its questions much earlier than if it had to create one comprehensive prototype

#### Analytical vs Physical
![[Pasted image 20240513231635.png]]


#### Comprehensive vs Focused
![[Pasted image 20240513231659.png]]


#### Phase 5 - Production ramp-up
- In the production ramp-up phase, the product is made using the intended production system
- The purpose of the ramp-up is to train the work force and to work out any remaining problems in the production processes
- Products produced during production ramp-up are sometimes supplied to preferred customers and are carefully evaluated to identify any remaining flaws

#### What is ‘Robust Design’
- A robust product is one that has robust performance, i.e. it performs as intended even under non-ideal conditions
    - e.g. manufacturing variations, varying operating conditions
- Robust design is the product development activity of creating a robust product
- We need to carry out tests or experiments at various stages in the design process to help us create this robust product

- For a given performance target, many combinations of parameter values can give us the desired result
    - e.g. you can compensate for a mobile phone case attenuating the radio signal by increasing the gain of the RF amplifier
- Some of these parameters are more sensitive to uncontrolled variables than others
- We need to choose the set of parameters that gives us the lowest overall sensitivity and meets all of our design criteria
- This is known as a robust setpoint

##### Where does this happen in product development?
- The earlier that robustness can be considered in product development, the better the results
- Robust design experiments can be used in concept development to refine the specifications
- Used most frequently during the detail design phase to make sure that we get the required product performance under a variety of conditions

![[Pasted image 20240513233306.png]]

#### Parameter values and variation
- A specific amplifier current may give us a specific gain
- However, the value of that current may vary from its nominal value due to, e.g., power supply manufacturing variations
- This will result in us seeing some variability in the RF gain

![[Pasted image 20240513233604.png]]


##### The Sensitivity of Setpoints
- The strength of the RF signal is, for example, a function of the gain and the attenuation
- We would choose setpoints based on a combination of values that gave the right strength and least variation

![[Pasted image 20240513233645.png]]
