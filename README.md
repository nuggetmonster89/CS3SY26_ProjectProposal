# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:
### Project Title or Name of the Application	: BeepBolt: A faster and accessible Beep Card System
### Section			   	      : 9-Sodium
### Group Members			    : 
    OROZCO, Tiffany Aviella B.
    TAMBABA, Amber Yphan SP.
    TISOY, Zasha Jozelle
### Date (Proposal Date)  : Nov 18, 2026
### Project Description: Project description is below.

- A brief summary of the project description and the need for it.
Our project aims to provide an alternate, more efficient way to improve the daily commuting experience for civilians. With features similar to a credit card (Deposit & Withdraw), our Beep Card offers a faster process in commuting. Along with this, it also takes into account the Student Discount, PWD Discount, and Senior Discount when using the card to pay for your ticket. In a country where public transportation is still developing, this approach is one of the many possible solutions the commuting civilian needs in order for a more peaceful experience when commuting.

- Describes system components, features, and expected outputs clearly and logically. NOTE: Clearly described the elements(classes), their attributes and methods and how they will interact with each other.
The code will have 4 main features: depositing money (deposit_cash), withdrawing money (withdraw_cash), paying for a ticket (fare_payment), and calculating the amount to pay after a discount is applied (apply_discount). The first class is the BeepCard class, which serves as the parent class for the three types of cards: StudentCard, PWDCard, and SeniorCard. It contains the basic attributes such as the person's name, card number, and remaining balance while also having the methods deposit_cash(), withdraw_cash(), and fare_payment(), which allow users to manage their money and pay for their fares. The StudentCard, PWDCard, and SeniorCard classes inherit the attributes and methods of the BeepCard class. Each subclass has additional attributes that identify the owner's eligibility for a discount. The StudentCard class includes the student's LRN, school name, and student discount. The PWDCard class contains the PWD ID number, disability type, and corresponding PWD discount. Meanwhile, the SeniorCard class includes the senior card number and senior discount. All three subclasses have an apply_discount() method that calculates the final, reduced fare based on the cardholder's eligibility. The next main class is the Vehicle class, which is the parent class of the Train, Car, and Bus classes, containing attributes such as the vehicle company, base fare, and number of stops passed and methods calculate_fare() and fare_payment(), which are responsible for calculating the passenger's fare and processing the payment. The Train, Car, and Bus classes inherit from the Vehicle class, each having additional attributes depending on the type of transportation. The Train class includes the train line and base fare. The Car class contains the service provider, plate number, rush-hour multiplier, distance travelled, and base fare, which are used to calculate its fare. Lastly, the Bus class includes the bus line, base fare, and number of stops passed. Both the Train and Car classes have a calculate_fare() method, while the Bus class has both calculate_fare() and fare_payment() methods. When a passenger uses their BeepCard, the system identifies the type of card they have and determines whether they are eligible for a discount. The selected vehicle's class then calculates the original fare based on its corresponding attributes. If the passenger qualifies for a discount, the appropriate card subclass applies the discount to the calculated fare. Finally, the BeepCard processes the payment by deducting the final fare from the user's available balance. The expected outputs include the calculated fare, final amount to be paid, payment conifmration message, and updated card balance.

- Include the description as well of your target demographics as the user of your application. 
The primary target demographics of this system are civilians who regularly commute in the Philippines. This would include students, working individuals, and daily commuters who want a more convenient way to pay their fares without carrying cash or worrying about having the exact payment. This system also caters to senior citizens and Persons with Disabilities (PWDs) by providing designated card types that account for their respective fare discounts, promoting inclusivity and making public transportation payments more accessible and efficient.

- The description is then followed by the class diagram, depicting clearly what was described.
https://canva.link/1tlvfxwbpgbohpg

**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

### Goals:

Describe the long term outcomes of your project followed by a couple of objectives to meet the goals stated in this paragraph.
With a more efficient commuting system, we’ll be able to elevate the daily public transportation to a smoother, faster experience. Along with the efficient aspect, it’ll also make commuting easier for seniors, PWDs, and also the minority that have a hard time interacting with other people especially in such a rushed environment. On the other hand, it’ll also make managing finances & accounting much more systematic and narrows down the chances of any discrepancies. To achieve this, we could begin with implementing the project in certain populated areas to see how it would perform in the real setting. Depending on the results, we will continuously implement the project across the region until the people have adjusted and learnt how the system works. Through this approach, we can slowly introduce the project to the people without any trouble, and account for any errors that will be changed as more of the project gets installed throughout the area.

- Objective 1: Reduce average commuting time of Filipino Citizens situated in Metro Manila by at least 15% by reducing the fare payment process to a single Beep card tap.
- Objective 2: Cut fare-discount application errors and bias by automating Student, Senior Citizen, and PWD validation and every transaction to be audited.
- Objective 3: Integrate the beep card system to at least 10 independent car & transport operators with around 95% transaction success rate.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
