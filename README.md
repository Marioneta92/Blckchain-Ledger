# Blckchain-Ledger
![image](https://user-images.githubusercontent.com/114365472/224849918-b928e296-e638-4e93-a90a-2aef8e3a2466.png)

Background

You’re a fintech engineer who’s working at one of the five largest banks in the world. You were recently promoted to act as the lead developer on their decentralized finance team. Your task is to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger will allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.
What You're Creating

You’ll make the following updates to the provided Python file for this Challenge, which already contains the basic PyChain ledger structure that you created throughout the module:

    Create a new data class named Record. This class will serve as the template for the financial transaction records that the blocks of the ledger will store.

    Change the existing Block data class by replacing the generic data attribute with a record attribute that’s of type Record.

    Create additional user input areas in the Streamlit application. These input areas will collect the relevant information for each financial record that you’ll store in the PyChain ledger.

    Test your completed PyChain ledger.

Instructions

Open the provided pychain.py file, which you’ll use to complete the steps for this Challenge. Notice that the PyChain ledger that you built throughout this module already includes the functionality to create blocks, perform the proof of work consensus protocol, and validate blocks in the chain.

The steps for this Challenge are divided into the following sections:

    Create a Record Data Class

    Modify the Existing Block Data Class to Store Record Data

    Add Relevant User Inputs to the Streamlit Interface

    Test the PyChain Ledger by Storing Records

Step 1: Create a Record Data Class

Define a new Python data class named Record. Give this new class a formalized data structure that consists of the sender, receiver, and amount attributes. To do so, complete the following steps:

    Define a new class named Record.

    Add the @dataclass decorator immediately before the Record class definition.

    Add an attribute named sender of type str.

    Add an attribute named receiver of type str.

    Add an attribute named amount of type float.

    note

    You’ll use this new Record class as the data type of your record attribute in the next section.

Step 2: Modify the Existing Block Data Class to Store Record Data

Rename the data attribute in your Block class to record, and then set it to use an instance of the new Record class that you created in the previous section. To do so, complete the following steps:

    In the Block class, rename the data attribute to record.

    Set the data type of the record attribute to Record.

Step 3: Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the Block record. To do so, complete the following steps:

    Delete the input_data variable from the Streamlit interface.

    Add an input area where you can get a value for sender from the user.

    Add an input area where you can get a value for receiver from the user.

    Add an input area where you can get a value for amount from the user.

    As part of the Add Block button functionality, update new_block so that Block consists of an attribute named record, which is set equal to a Record that contains the sender, receiver, and amount values. The updated Blockshould also include the attributes for creator_id and prev_hash.

Step 4: Test the PyChain Ledger by Storing Records

Test your completed PyChain ledger and user interface by running your Streamlit application and storing some mined blocks in your PyChain ledger. Then test the blockchain validation process by using your PyChain ledger. To do so, complete the following steps:

    In the terminal, navigate to the project folder where you've coded the Challenge.

    In the terminal, run the Streamlit application by using streamlit run pychain.py.

    Enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger.

    Verify the block contents and hashes in the Streamlit drop-down menu. Take a screenshot of the Streamlit application page, which should detail a blockchain that consists of multiple blocks. Include the screenshot in the README.md file for your Challenge repository.

    Test the blockchain validation process by using the web interface. Take a screenshot of the Streamlit application page, which should indicate the validity of the blockchain. Include the screenshot in the README.md file for your Challenge repository.
    
The Following is a Snapshot/Screenshot of the streamlit Application.
![image](https://user-images.githubusercontent.com/114365472/224853192-0d248d0b-4762-484b-805d-a7a368abb9b6.png)

. The streamlit Application Simulates a Blockchain- Based Ledger system that allows users to conduct financial transsactions like tranfers of funds from sender to receiver, and to verify the integrity of the data.

1. Use of Application: the user is prompted to enter a sender Address, the Receiver Address and the amount of crypto send.
2. Ledger: the ledger than Tracks and stores the transactions in which the user is able to inspect each Block transaction with the use of a "BLOCK iNSPECTOR" option located on the Left Drop-down menu of the Application.
3. Evaluate Ledger: the user can then click on the option "VALIDATE CHAIN" to compare the Hash of the previous block of the previous Hash of the current block.




