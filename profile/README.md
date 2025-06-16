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
    A[Ryujin Agent] --> B{TCP Connection}
    B -->|Success| C[Send Registration Request]
    B -->|Failed| D[Connection Failed]
    C --> E[Manager: Validate Password]
    E -->|Valid| F[Generate Certificates]
    E -->|Invalid| G[Reject Registration]
    F --> H[Send Credentials to Agent]
    H --> I[Agent: Store Certificates]
    I --> J[Start Heartbeat Loop]
    J --> K[Send Heartbeat Every 5s]
    K --> L[Manager: Update Agent Status]
    L --> M{Agent Active?}
    M -->|Yes| N[Continue Monitoring]
    M -->|No| O[Mark as Disconnected]
    N --> P[Collect System Data]
    P --> Q[File Integrity Monitoring]
    P --> R[System Inventory Collection]
    P --> S[Security Event Detection]
    Q --> T[Send FIM Data]
    R --> U[Send Inventory Data]
    S --> V[Send Security Events]
    T --> W[Manager: Process Data]
    U --> W
    V --> W
    W --> X[Store in Database]
    X --> Y[WAF Processing]
    Y --> Z[Dashboard Display]
    Z --> AA[User Interface]
    
    subgraph "Agent Components"
        P
        Q
        R
        S
    end
    
    subgraph "Manager Components"
        E
        F
        L
        W
        X
        Y
    end
    
    subgraph "Dashboard Components"
        Z
        AA
    end
```

All projects are created by Ryan Rizky Pratama & Reja Revaldy F 
