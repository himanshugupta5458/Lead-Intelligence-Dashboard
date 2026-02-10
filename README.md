# Lead Intelligence Dashboard 🏢

> Built to solve a ₹1-2 Cr annual Google Ads spend optimization problem in India's premium real estate sector

![Dashboard Preview](https://img.shields.io/badge/Status-Production-brightgreen)
![Python](https://img.shields.io/badge/Python-3.9+-blue)
![React](https://img.shields.io/badge/React-18+-61DAFB)



https://github.com/user-attachments/assets/11e29077-a7e6-4832-8b25-c6948ae53145



## 🎯 Business Context

Built this system while working full-time at one of Google's largest real estate advertising clients in India. The company was spending **₹1-2 Crore monthly** on Google Ads with severely broken tracking systems.

### The Real Estate Challenge

In premium real estate, the economics are brutal:
- **₹8,000-10,000 cost per lead** (CPL) is normal
- High-ticket products (₹50L-5Cr properties) require precision targeting
- Single bad campaign = ₹2-3 lakhs wasted before anyone notices
- Sales cycles span 3-6 months, making attribution nearly impossible

When I joined, the company had:
- ❌ Zero visibility into which campaigns drove actual site visits or bookings
- ❌ No way to identify fraud/junk leads draining budget
- ❌ Marketing and sales operating on completely different data
- ❌ 3-4 week lag between spending and realizing a campaign was broken

## 💰 The Cost Problem

### What We Were Facing

**Monthly Ad Spend**: ₹1-2 Crore  
**Cost Per Lead**: ₹8,000-10,000  
**Problem**: ~30% of leads were junk (wrong phone numbers, fake inquiries, bot traffic)  
**Impact**: ₹30-60 Lakhs wasted monthly on worthless leads

**Specific Issues Discovered:**
1. **Fraudulent Lead Farms**: Multiple "leads" coming from same IP addresses
2. **Wrong Audience Targeting**: Campaigns reaching people who couldn't afford properties
3. **Google's Black Box**: Their algorithm optimized for "conversions" (form fills) not quality
4. **No Feedback Loop**: Sales data never reached Google Ads for optimization

## ✅ What This System Solved

### 1. **Junk Lead Detection** 
**Problem**: Paying ₹10K for leads from the same IP submitting fake details  
**Solution**: Built IP tracking and pattern recognition to flag suspicious activity  
**Result**: Identified and blocked ₹8-12 lakhs monthly in fraud

### 2. **Sales Data Feedback to Google Ads**
**Problem**: Google optimized for form submissions, not actual buyers  
**Solution**: Integrated CRM data back into Google Ads as "offline conversions"  
**Result**: Google's algorithm learned what a real buyer looks like  
**Impact**: 23% reduction in CPL over 3 months

### 3. **Campaign Quality Visibility**
**Problem**: Waited weeks to realize a campaign was burning money  
**Solution**: Real-time dashboards showing lead-to-site-visit conversion  
**Result**: Bad campaigns identified in 48 hours instead of 3 weeks

### 4. **Marketing-Sales Alignment**
**Problem**: Marketing celebrated 200 leads/month, Sales said only 40 were serious  
**Solution**: Single dashboard showing MQL→SQL→Site Visit→Booking funnel  
**Result**: Both teams now optimize for "qualified leads," not just volume

## 📊 Business Impact

### Measurable Outcomes

| Metric | Before | After | Impact |
|--------|--------|-------|--------|
| **Cost Per Lead** | ₹10,200 | ₹7,850 | ↓ 23% |
| **Junk Lead %** | 32% | 11% | ↓ 65% |
| **Monthly Waste** | ₹35L | ₹12L | **₹23L saved/month** |
| **Time to Identify Bad Campaign** | 5-7 days | 2 days | ↓ 70% |
| **Lead-to-Site-Visit Rate** | 12% | 19% | ↑ 58% |

**Annual Savings**: ~₹2.7 Crore from waste elimination and CPL reduction

### Strategic Wins

✅ **Became Data-Driven**: Decisions backed by attribution data, not gut feel  
✅ **Faster Iteration**: Test new campaigns with 2-day feedback vs 3-week blind period  
✅ **Better Google Performance**: Offline conversion data improved algorithm targeting  
✅ **Team Alignment**: Marketing and sales finally spoke the same language

## 🔍 Key Features Built

### Core Capabilities

**1. Lead Quality Tracking**
- MQL → SQL → Site Visit → Booking funnel visibility
- Lead source attribution (campaign, keyword, ad)
- Cost per stage calculation (cost per site visit, cost per booking)

**2. Fraud Detection**
- IP address pattern analysis
- Duplicate lead detection (same phone/email from multiple sources)
- Suspicious submission time patterns
- Geographic anomaly detection

**3. Google Ads Integration** 
- Automated offline conversion uploads
- Campaign performance by quality (not just volume)
- Cost per qualified lead vs cost per raw lead
- ROAS calculation based on actual bookings

**4. Real-Time Alerts**
- Campaign quality degradation warnings
- Junk lead spike notifications  
- Budget efficiency alerts
- High-value lead notifications to sales

**5. Executive Dashboards**
- Monthly spend vs qualified lead trends
- Channel-wise ROAS comparison
- Sales cycle length by source
- Revenue attribution reports

## 🛠️ Tech Stack

**Frontend**: React + TypeScript + Tailwind CSS + shadcn/ui  
**Backend**: Python FastAPI + SQLAlchemy  
**Database**: PostgreSQL (production), SQLite (demo)  
**Integrations**: Google Ads API, Salesforce API  
**Deployment**: AWS (EC2 + RDS)


## 💡 Lessons Learned

**1. Integration is Everything**: The dashboard was only valuable once CRM and Google Ads data flowed automatically. Manual exports = system dies.

**2. Fraud is Rampant**: In high-CPL industries, lead farms and click fraud are significant. Built-in fraud detection isn't optional.

**3. Feedback Loops Win**: Sending sales data back to Google Ads had more impact than any campaign optimization technique.

**4. Align Metrics First**: Unified dashboards only work if marketing and sales agree on definitions (what is an SQL? what counts as qualified?).

**5. Speed Matters**: Real-time data turned a 3-week decision cycle into 2 days. Competitive advantage in ad buying.


