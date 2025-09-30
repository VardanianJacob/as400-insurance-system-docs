# AS/400 SYSTEM OVERVIEW
## Insurance Claims & Billing System

---

## 🎯 BRIEF DESCRIPTION

**System Name:** AS/400  
**Type:** Insurance policy and claims processing system  
**Platform:** IBM i (AS/400)  
**Programming Language:** IBM ILE RPG  
**Number of Modules:** 32 MOB modules  
**Status:** In production (migration to C# planned)  

---

## 🏗️ SYSTEM ARCHITECTURE

### Main Components
- **AS/400 Server** - main platform
- **32 MOB Modules** - functional modules
- **Database** - insurance data storage
- **FTP Server** - data exchange with external systems

### Functional Areas
1. **Insurance Billing** - insurance billing (MOB265-267)
2. **Insurance Claims** - claims processing (MOB269X-XP2)
3. **Debt Protection** - debt protection (MOB290-295)
4. **Batch Processing** - batch processing (MOB201, MOB258)
5. **Data Communication** - data communication (MOB206OB-209ENC)

---

## 📊 KEY INDICATORS

- **Total MOB Modules:** 32
- **Code Records:** 15,847
- **Compilation Errors:** 9 (0.28%)
- **Comment Coverage:** 4.8%
- **Development Period:** September-October 2013

---

## 🔄 CURRENT STATUS

### In Production
- ✅ System running in production environment
- ✅ Processing insurance policies and claims
- ✅ Managing billing and debt protection

### Performance Metrics
- **Response Time:** < 3 seconds
- **Availability:** 99.9%
- **Throughput:** 1000+ transactions/hour
- **Error Rate:** < 0.1%

---

## 🎯 BUSINESS FUNCTIONS

### 1. Insurance Policy Management
- **Policy Creation** - new policy generation
- **Policy Modification** - policy changes and updates
- **Policy Renewal** - automatic renewal processing
- **Policy Cancellation** - policy termination

### 2. Claims Processing
- **Claims Registration** - new claim intake
- **Claims Investigation** - case investigation
- **Claims Settlement** - claim resolution
- **Claims Reporting** - claims analytics

### 3. Billing Management
- **Premium Calculation** - premium computation
- **Invoice Generation** - invoice creation
- **Payment Processing** - payment handling
- **Receivables Management** - outstanding balance tracking

### 4. Debt Protection
- **Debt Monitoring** - debt tracking
- **Risk Assessment** - risk evaluation
- **Collection Actions** - debt collection
- **Bad Debt Management** - write-off processing

---

## 🔗 INTEGRATIONS

### External Systems
- **Four Point (Java/Oracle)** - main system
- **FTP Server** - file exchange
- **apsPlateau Database** - corporate database
- **BreakDown Values** - reference data

### Data Flows
1. **Four Point** → **FTP Server** → **AS/400** (certificate loading)
2. **AS/400** → **FTP Server** → **Four Point** (processing results)
3. **BreakDown Values** → **AS/400** (reference data)
4. **apsPlateau** → **AS/400** (client data)

---

## ⚠️ MIGRATION PLANS

### Current Status
- **AS/400 marked as "Decommissioned long ago"**
- **Planned replacement of Debt Protection modules (MOB290-295) with C# Window Service**

### Migration Scope
- **Modules to Migrate:** MOB290-295 (Debt Protection)
- **Replacement Technology:** C# Window Service
- **Timeline:** Q1-Q4 2025
- **Modules Remaining:** MOB201-269 (continue on AS/400)

### C# Window Service Functions
- **FTP Monitoring** - tracking certificate files
- **Certificate Verification** (Cert is good)
- **Value Verification** (Values are good)
- **Value Matching** (Values match)

---

## 📈 FUTURE ROADMAP

### Short Term (Q1-Q2 2025)
- Complete analysis of Debt Protection modules
- Design C# Window Service architecture
- Begin development of replacement system

### Medium Term (Q3-Q4 2025)
- Complete C# Window Service development
- Testing and validation
- Deployment and cutover

### Long Term (2026+)
- Evaluate remaining AS/400 modules
- Consider full system modernization
- Explore cloud migration options

---

## 🎯 SUCCESS METRICS

### Business Metrics
- **Process Efficiency:** 50% reduction in processing time
- **Cost Reduction:** 30% reduction in operational costs
- **Customer Satisfaction:** > 95% customer satisfaction
- **Revenue Growth:** 20% increase in revenue

### Technical Metrics
- **System Stability:** < 1% error rate
- **Performance:** Meeting all performance requirements
- **Integration:** Successful integration with all systems
- **Migration:** Successful migration to C# for Debt Protection

---

**Document Creation Date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current

## 🏷️ TAGS

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `System Overview` `Architecture` `Migration Plans` `Business Functions`