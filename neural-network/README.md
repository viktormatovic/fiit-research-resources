# Expected pattern sequences

From experiment 1:

1. Subclass Per Team (p=0.799468) -> Patron Role (p=0.674086) -> Hierarchy of Factories (p=0.147888). 
This pattern sequences introduces experienced person to decide when is the right place to optimize hierarchies of classes into the Hierarchy of Factories design pattern. This pattern sequence is established from patterns in People and Code Pattern Language and Piecemeal Growth Pattern Language. This pattern sequence was established using explicit relationship (Hierarchy of Factories implements Subclass Per Team) and implicit relationship between its patterns.
3. Private Versioning (p=0.942623) -> Phasing it in (p=0.731583) -> Generics and Specifics (p=0.436626). 
This pattern sequence can be used to implement solution expected to be used across many software projects. Private Versioning pattern starts this sequence because of the need to experiment with new technology. Once the stable developer is ready, new experienced developer comes up by developing generic framework with UI components. These UI components are being put together by the stable though less experienced developer into the application-specific solution. This application-specific solution is a proof of concept for other software projects waiting to be integrated with this solution in the future.
4. Architect Also Implements (p=0.998732) -> Standup Meeting (p=0.066231) -> Architecture Team (p=0.058503). 
This pattern sequence was seen when more experienced lead developer (architect) worked on the first version of the software module with the less experienced through the use of the generic sub-modules customized in one application as the proof-of-concept. They worked with new technology in the company and formed the Architecture Team. They discussed the progress in the project in Standup Meetings ocassionally joined by project manager.
5. Distribute Work Evenly (p=0.060515) -> Hierarchy of Factories (p=0.057696) -> Generics and Specifics (p=0.057791)
This pattern sequence can be used to implement the software library shared by multiple applications where modules of the library are implemented with novices given the requirements for these modules from experts. Use of this library by numerous other applications is possible due to the genericity of the library.

From experiment 2:
1. Architect Controls Product (p=0.228964) -> Few Roles (p=0.126118) -> Code Ownership (p=0.119162)
This pattern sequence documents usual setting in software house companies, where skilled and experienced developer is assigned application owner role. He still can have consultants assigned or it's own developer to help, but everything flows through the owner hands.
2. Generics and Specifics (p=0.562330) -> Distribute Work Evenly (p=0.356492) -> Architect Controls Product (p=0.238690). This pattern documents situation where framework and possibly its application in another code base or product is developed and maintained by various roles. Build of the final product is supervised by architect who directs the architectural style of this framework.
3. Architect Also Implements (p=0.995495) -> Code Ownership (p=0.061411) -> Lock Em Up Together (p=0.059739)
This pattern sequence clearly documents how architecture is designed and developed by the consistent team led by lead developer who is an architect and who directs the architectural style of the product.
4. Developing In Pairs (p=0.055370) -> Distribute Work Evenly (p=0.054725) -> Architecture Team (p=0.051247)
This pattern sequence documents how the system is developed. Developers write the code (Developing In Pairs). Because they want to conduct code review as soon as possible and because some developers are more skilled and experienced than the others, they write the code in pairs. Developers are organized into small groups (or even one group, one pair) headed by architects of the partitions. System is partitioned and it's architecture is designed by high level architects because of the application of Architecture Team organizational pattern.

# How to use

Install Python and Jupyter Notebook or Jupyter Lab. Then run from this place as ```jupyter notebook```. Your app is then accessible at ```http://localhost:8889/?token=<your-token>```.

ANN is MLP and is implemented in Python 3.8.0, with TensorFlow: https://www.tensorflow.org/ and Keras: https://keras.io/. Keras is a handy facade of TensorFlow for those who don't want to work with a low-level API.

Dependencies:

- latest pip as Python's dependency manager, see https://pypi.org/project/pip/
- tensorflow for neural network API, see https://www.tensorflow.org/
- sklearn for data wrangling, see https://scikit-learn.org/stable/
- numpy for data wrangling, see https://numpy.org/
- pandas for data wrangling, see https://pandas.pydata.org/
- matplotlib for evaluation: see https://matplotlib.org/

# Why we should use artificial neural networks to search for implict relationships between organizational patterns?

Simply because they are one of the most efficient techniques how we can encode information about the real world
in its artificial representation. We encode this information in hidden layers of the artificial neural network. 
This is one of the accepted techniques which allows us to learn artificial representations of patterns. Learned representations
are widely considered to be much more efficient than a hand-crafted representations (e.g. with Prolog or through 
other languages for building knowledge base.)

# Why do we need to use multiple-layer artificial neural networks to search for implicit relationships between organizational patterns?

Each of the layers represent information about the pattern in some level. Combination of layers together enables us
solve our problem. Thus we try to solve our problem by decomposing bigger problem to its smaller parts - layers of the ANN.
Almost all ML techniques can be transformed to their neural network representation (ANN with 3 layers max.)

# Why we should use deep learning techniques instead of the machine learning techniques?

Deep learning techniques allow us to solve tasks which cannot be solved with simple machine learning techniques. 
They allow us to represent information about the processes described in organizational patterns and learn these
representations automatically. This means to automatically enhance them to have better representations.

Convolutional Neural Networks are a great way how we can search for patterns as flexibly as we can. Convolutional
Neural Networks can be used to connect multiple patterns to create bigger whole, because of their ability to search
for global tendencies. Multiple-layer perceptrons, in the other hand, can be only used to search for local tendencies.

See more about the CNN if you're interested here https://d2l.ai/chapter_convolutional-neural-networks/index.html

# Why do we talk about the multi-layer perceptrons instead of the neurons or perceptrons?

Logical neuron originally designed by Pitts & McCulloch in 1943 works only with integer or with binary-encoded attributes.
Their logical neuron also assumes that all attributes in a dataset have a same weight. In our case, this would mean
that all n-grams for some organizational pattern in a matrix of Waseeb et al. in 'Extracting Relations Between
Organizational Patterns Using Association Mining' on page 4. Table 1 would contribute same to the final output
of our probability model. Activation function for this logical neuron creates another problem for us. It does
not exhibit information ahead through the network if sum of the n-gram incidents is not bigger than some predefined threshold T.

# What is the biggest advantage of ANN and deep learning techniques? Why we should use these techniques here?

Artificial neural networks allow us to generalize and abstract information we find in the study of organizational
patterns. Deep learning techniques allow us to learn these representations and enhance them. 
