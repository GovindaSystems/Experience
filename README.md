# Experience

<p align="center">
    <img src="assets/logo.jpg" height="25%" width="25%" alt="Unform" />
</p>

> Experience is:

* A decentralized e-commerce platform empowering individuals to create their own stores and sell products effortlessly.

Registration:
    
    - Store 
    - Products 

* A community-driven engagement tool:

Modules:

    - Cashback - utilizing its native currency - (backing)
    - Promotion - Products / Coupons / Commissions (product/123?seller=ABC) [Ambassador / Promoter]
    - SEO for organic / paid traffic (enhancing store / product / showcase visibility / ...)

* Consulting service and personalized support for Companies / Entrepreneurs (School & Consulting)

    - Consultancy to enhance the user experience with your product
    - Presentation consultancy (service / product)
    - Economic viability analysis (service / product) (clarity for the scenario)

Experience is an innovative platform aiming to assist merchants in offering products and services intelligently and efficiently in a decentralized, community-driven environment. Inspired by the TV series "Fantasy Island," the platform allows customers to live out their fantasies and dreams through unique and personalized experiences. Here, merchants can register unique experiences that customers can enjoy, creating a decentralized ecosystem of service and product exchange.

---

## Mission

Our mission at Experience is to create a decentralized space where merchants can offer unique and memorable experiences to their customers. We want to facilitate the connection between people and experiences, allowing customers to discover new ways to enjoy life and merchants to expand their businesses efficiently and innovatively within a DAO-based model.

---

## Vision

Our vision is to be the leading decentralized platform connecting people to unique and innovative experiences worldwide. We aim to be recognized as a community that values quality, innovation, and collaboration between merchants and customers within a DAO framework.

---

## Purpose

Our purpose is to enrich people's lives through memorable experiences in a decentralized and community-driven manner. We believe that each experience is an opportunity to learn, grow, and connect with others. We want every customer who uses Experience to feel that their life has been enriched in some way within the decentralized ecosystem.

---

## Customer

Our customers are curious and adventurous individuals who are always looking for new experiences to enrich their lives. They value quality, authenticity, and innovation, and are always ready to try something new within the decentralized framework.

---

## Supplier

Our suppliers are passionate and talented merchants who are eager to share their unique experiences with the world. They are innovators, creative, and committed to excellence in everything they do within the DAO framework.

---

## Kind Organizers (Promoter)

Our kind organizers are the facilitators who make everything possible within our decentralized ecosystem. They are responsible for ensuring that each experience is perfectly organized and managed, and that each customer leaves satisfied.

---

## About Experience

Experience is more than a platform; it's a decentralized community. Here, merchants of all kinds can offer amazing experiences to their customers in a decentralized and community-driven environment. Whether it's a gourmet dinner, a sightseeing tour, a dance class, a craft beer tasting, or any other experience you can imagine, Experience is the place to share it.

---

## How Experience Works

Experience is designed to help you, the merchant, create, organize, and manage the best experiences your customers can have within a decentralized ecosystem. With your talent and our decentralized organization, the sky is the limit. Through our platform, you can manage your offerings, track customer interest, and receive valuable feedback that can help further improve your experiences within the DAO model.

## User Journeys

Initial journey, unregistered user:

```mermaid
graph TD
    A[Home] --> B[Choose product]
    B --> C[User registration]
    C1[Metamask]
    C2[E-mail]
    C3[Social Network]
    C --> C1
    C --> C2
    C --> C3
    C --> D[Payment method registration]
    D1[Pix]
    D2[Card]
    D3[Bitcoin]
    D4[Cash Back]
    D5[Invoice]
    D --> D1
    D --> D2
    D --> D3
    D --> D4
    D --> D5
    D --> E[Delivery address registration]
    E --> F[Review cart]
    F1[Payment]
    F2[Delivery address]
    F3[Payment method]
    F --> F1
    F --> F2
    F --> F3
    F --> G[Success payment approved]
    F --> H[Payment error]
```


### 1. Register a user

```mermaid
sequenceDiagram
    participant User
    participant ExperiencePlatform
    
    User ->> ExperiencePlatform: Access registration page
    ExperiencePlatform -->> User: Display registration form
    User ->> ExperiencePlatform: Fill in registration details
    ExperiencePlatform -->> User: Verify and create user account
```

### 2. How to register a store

```mermaid
sequenceDiagram
    participant Merchant
    participant ExperiencePlatform
    
    Merchant ->> ExperiencePlatform: Log in to merchant account
    ExperiencePlatform -->> Merchant: Display merchant dashboard
    Merchant ->> ExperiencePlatform: Navigate to "Add New Store"
    ExperiencePlatform -->> Merchant: Show store registration form
    Merchant ->> ExperiencePlatform: Fill in store details
    ExperiencePlatform -->> Merchant: Verify and create store
```

### 3. How to add products

```mermaid
sequenceDiagram
    participant Merchant
    participant ExperiencePlatform
    
    Merchant ->> ExperiencePlatform: Log in to merchant account
    ExperiencePlatform -->> Merchant: Display merchant dashboard
    Merchant ->> ExperiencePlatform: Select the desired store
    ExperiencePlatform -->> Merchant: Show store management interface
    Merchant ->> ExperiencePlatform: Choose "Add New Product"
    ExperiencePlatform -->> Merchant: Show product registration form
    Merchant ->> ExperiencePlatform: Fill in product details
    ExperiencePlatform -->> Merchant: Verify and add product to the store
```

### 4. How to set up payment methods (Bitcoin, PIX, Credit Card)

```mermaid
sequenceDiagram
    participant Merchant
    participant ExperiencePlatform
    participant PaymentProvider
    
    Merchant ->> ExperiencePlatform: Log in to merchant account
    ExperiencePlatform -->> Merchant: Display merchant dashboard
    Merchant ->> ExperiencePlatform: Navigate to "Payment Settings"
    ExperiencePlatform -->> Merchant: Show payment settings interface
    Merchant ->> ExperiencePlatform: Select "Add Payment Method"
    ExperiencePlatform -->> Merchant: Display available payment options
    Merchant ->> ExperiencePlatform: Choose payment method (Bitcoin, PIX, Credit Card)
    ExperiencePlatform ->> PaymentProvider: Redirect to payment provider for configuration
    PaymentProvider -->> ExperiencePlatform: Return confirmation of configuration
    ExperiencePlatform -->> Merchant: Confirm successful payment method setup
```

---

## Architecture

```mermaid
graph TD;

subgraph "Blockchain"
    Web3((IoTeX Smart Contract)) -- Transactions / Coin / Cashback --> FE
end

subgraph "Client Side"
    FE(Vercel) -- Web3 Integration --> Web3
    FE -.-> MongoDB
end

subgraph "Server Side"
    MongoDB((MongoDB)) -- Data Storage --> FE
    MongoDB -- Data Storage --> BE
    BE[Server] -- Data Processing --> MongoDB
    BE -- IoTeX Integration --> Web3
end
```

In this decentralized architecture:

- **FE (Vercel)** represents the frontend hosted on Vercel.
- **Web3** represents the integration with Web3 for interacting with IoTeX smart contracts.
- **MongoDB** is used for data storage and is accessed by both the frontend and backend.
- **BE (Server)** represents the decentralized backend server, interacting with MongoDB and integrating with IoTeX through Web3 for transactions and other blockchain-related functionalities.

---

## Timeline

```mermaid
gantt
    title Project Delivery Schedule

    dateFormat  YYYY-MM-DD
    axisFormat %m/%d

    section Project Phases
    Defining_Requirements :done, Defining Requirements, 2023-09-01, 2023-09-15
    Creating_Screen_Prototype :done, Creating Screen Prototype, 2023-09-16, 2023-09-30
    Development_Home_Page :done, Development of Home Page, 2023-10-01, 2023-10-15
    Product_Registration_Development : Product Registration Development, 2023-10-16, 2023-10-31
    Store_Registration_Development : Store Registration Development, 2023-11-01, 2023-11-15
    Promoter_Registration_Development : Promoter Registration Development, 2023-11-16, 2023-11-30
    Commission_Functionality_Development : Commission Functionality Development, 2023-12-01, 2023-12-15
    Google_Social_Login_Development : Google/Social Login Development, 2023-12-16, 2023-12-31
    Other_Payment_Methods_Development : Other Payment Methods Development, 2024-01-01, 2024-01-15
```

- 1 - Requirement Definition (Status: Done)
- 2 - Screen Prototype Creation (Status: Done)
- 3 - Development of Home page / Login via metamask / Products / Purchase Flow (payment in ETH test) (Status: Done)
- 4 - Product Registration Development
- 5 - Store Registration Development
- 6 - Promoter Registration Development
- 7 - Commission Functionality Development
- 8 - Login Development via Google / Social Network
- 9 - Development of other payment methods (Pix, Card, Bitcoin)

## Join Our Decentralized Community

We are always looking for talented and passionate merchants to join our decentralized community. If you believe you can offer amazing experiences to your customers and want to be part of a collaborative network of merchants within a DAO framework, join us at Experience.

---

## Social Impact - Social and Environmental Projects

At Experience, we believe that everyone has the right to enjoy amazing experiences. That's why we are committed to supporting social and environmental projects that help make the world a better place. With every experience booked, a percentage is donated to projects that support needy communities and sustainability initiatives.

---

## Contact Us

For more information, please contact us through our website or send an email to [email].

---

Experience - With your talent and our decentralized organization, the sky is the limit.