# Ryujin Security 🐉

Ryujin Security security monitoring and management.

## Our Projects

### [Ryujin Manager](https://github.com/ryujin-security/ryujin-manager)
Core management service that handles agent communication and certificate management.
- 🔐 Secure agent registration
- 📜 Certificate management
- 🔄 Real-time monitoring
- 🛡️ TLS-encrypted communication

### [Ryujin Agent](https://github.com/ryujin-security/ryujin-agent)
Endpoint security and monitoring agent.
- 🔍 File Integrity Monitoring (FIM)
- 📊 System Inventory Collection
- 🔒 Secure Authentication
- 🖥️ Real-time System Monitoring

### [Ryujin Dashboard](https://github.com/ryujin-security/ryujin-dashboard)
Web interface for security monitoring and management.
- 📈 Real-time Monitoring
- 🎯 Event Visualization
- ⚙️ Configuration Management
- 📱 Responsive Design
  
```mermaid
graph TD
    subgraph "Agent"
        A[Ryujin Agent]
        I[Store Certificates]
        P[Collect System Data]
        Q[File Integrity Monitoring]
        R[System Inventory]
        S[Security Events]
    end
    
    subgraph "Manager"
        B{TLS Connection}
        C[Registration Request]
        E[Validate Password]
        F[Generate Certificates]
        G[Reject Registration]
        H[Send Credentials]
        L[Update Agent Status]
        M{Agent Active?}
        N[Continue Monitoring]
        O[Mark Disconnected]
        W[Process Data]
        X[Store in Database]
        Y[WAF Processing]
    end
    
    subgraph "Dashboard"
        Z[Display Data]
        AA[User Interface]
    end
    
    A --> B
    B -->|Success| C
    B -->|Failed| G
    C --> E
    E -->|Valid| F
    E -->|Invalid| G
    F --> H
    H --> I
    I --> L
    L --> M
    M -->|Yes| N
    M -->|No| O
    N --> P
    P --> Q
    P --> R
    P --> S
    Q --> W
    R --> W
    S --> W
    W --> X
    X --> Y
    Y --> Z
    Z --> AA
```

All projects are created by Ryan Rizky Pratama & Reja Revaldy F 
