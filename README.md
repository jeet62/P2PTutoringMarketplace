# P2P Tutoring Marketplace

![Screenshot 2024-08-27 154146](https://github.com/user-attachments/assets/c70f0305-73f0-4d46-83bd-34ee213df4aa)

## Vision

The P2P Tutoring Marketplace is a decentralized platform designed to connect tutors and learners directly, leveraging blockchain technology for secure and transparent interactions. Our vision is to empower individuals with the ability to easily find and engage with qualified tutors while ensuring fair and efficient transactions through smart contracts.

## Flowchart
```
![Flowchart](+-----------------+
| User Registration |
+-----------------+
         |
         v
+-----------------+
|  Profile Setup  |
+-----------------+
         |
         v
+-----------------+
| Search & Match  |
+-----------------+
         |
         v
+-----------------+
| Session Booking |
+-----------------+
         |
         v
+-----------------------------+
| Smart Contract Interaction |
+-----------------------------+
         |
         v
+-----------------+
| Session Execution |
+-----------------+
         |
         v
+---------------------+
| Feedback & Ratings |
+---------------------+
         |
         v
+---------------------+
| Dispute Resolution  |
+---------------------+
         |
         v
       +-----+
       | End |
       +-----+
)
```
**Flowchart Overview:**
1. **User Registration**: Users (tutors and learners) create accounts.
2. **Profile Setup**: Tutors list their subjects and availability; learners specify their tutoring needs.
3. **Search & Match**: Learners search for suitable tutors.
4. **Session Creation**: Tutors and learners initiate a session request.
5. **Smart Contract Execution**: Payments and session details are managed by smart contracts.
6. **Session Completion**: Tutors and learners complete their sessions.
7. **Feedback & Ratings**: Users provide feedback and rate each other.
8. **Dispute Handling**: Any disputes are resolved according to platform rules.

## Contract Address
The smart contract for the P2P Tutoring Marketplace is deployed on the Ethereum blockchain. The contract address is:
```
0x41400f284b58b2e6e445b993e4210736675b5d99
```
![Screenshot_27-8-2024_155012_opencampus-codex blockscout com](https://github.com/user-attachments/assets/c4b2df0f-6af6-466b-ad70-00ed631c92e6)

Please confirm this address on a blockchain explorer before engaging with it.

## Future Scope
1. **Multi-Language Support**: Extend the platform to support multiple languages to cater to a global audience.
2. **Mobile Applications**: Develop mobile apps for both iOS and Android for enhanced user experience.
3. **Advanced Matching Algorithms**: Implement machine learning to improve the accuracy of tutor-learner matches.
4. **Additional Payment Methods**: Integrate more payment options including various cryptocurrencies and traditional methods.
5. **AI-Enhanced Tutoring Tools**: Introduce AI-based tools to support interactive and personalized learning experiences.
6. **Certification System**: Add certification features for completed courses and tutoring sessions.

## Contract Code Overview
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract P2PTutoringMarketplace {

    // Struct to represent learner requests
    struct LearnerRequest {
        string subject;
        uint level;
        uint duration;
    }

    // Mapping of learner addresses to their requests
    mapping (address => LearnerRequest) public learnerRequests;

    // Event emitted when a new tutoring session is created
    event NewSession(address tutor, address learner, uint sessionId);

    // Function to create a new tutoring session
    function createSession(address tutor, address learner, uint sessionId) public {
        // Match tutor with learner based on their profiles and requests
        // ...

        // Emit event to notify of new session
        emit NewSession(tutor, learner, sessionId);
    }

    function completeSession(uint sessionId) public pure {
        // Placeholder function
    }

    // Function to get the tutor address from a session ID
    function getTutorFromSessionId(uint sessionId) public view returns (address) {
        // Placeholder function
    }

    // Function to get the learner address from a session ID
    function getLearnerFromSessionId(uint sessionId) public view returns (address) {
        // Placeholder function
    }
}
```

## Contract Details
0x41400f284b58b2e6e445b993e4210736675b5d99


We appreciate your interest and look forward to your feedback and collaboration to enhance the P2P Tutoring Marketplace!

---

Thank you for exploring our project. Together, we can create a more accessible and effective learning environment.
