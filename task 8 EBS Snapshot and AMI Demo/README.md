# TASK-8: Exploring EC2, EBS Snapshots & AMIs on AWS

> **Advanced AWS Storage & Instance Management Demo**  
> Comprehensive exploration of **EBS Snapshots** and **Amazon Machine Images (AMIs)** for enterprise-grade data preservation and system replication.

---

## 🎯 **Objective**

Master critical AWS concepts:
- **EBS Snapshot Creation & Restoration** - Block-level storage backup
- **AMI Generation & Deployment** - Complete system image replication  
- **Storage vs System Backups** - Understanding granular vs holistic approaches
- **Cross-Instance Data Portability** - Seamless data migration strategies

---

## 🔧 **Technical Implementation**

### **Phase 1: Base Infrastructure Setup**
**Launch Primary EC2 Instance**
- Configure baseline AWS compute environment
- Establish foundational EBS volume attachment

![alt text](image.png)
![alt text](image-1.png)

---

### **Phase 2: Data Injection & Preparation**
**SSH Connection & Data Population**
- Remote access establishment via SSH
- Custom data creation for backup validation

![alt text](image-2.png)

---

### **Phase 3: EBS Snapshot Operations**
**Block-Level Storage Backup**
- **Point-in-time snapshot creation**
- Volume-level data preservation
- **Incremental backup methodology**

![alt text](image-3.png)

---

### **Phase 4: Volume Restoration Process**
**Snapshot-to-Volume Conversion**
- New EBS volume provisioning from snapshot
- **Data integrity verification**
- Cross-AZ volume deployment capability

![alt text](image-4.png)
![alt text](image-5.png)

---

### **Phase 5: AMI Creation Workflow**
**System Image Generation**
- **Complete instance state capture**
- Boot volume + configuration preservation
- **Template creation for rapid deployment**

![alt text](image-6.png)

---

### **Phase 6: Cross-Platform Testing**
**RHEL Instance Deployment**
- Launch secondary EC2 instance (Red Hat Enterprise Linux)
- **Operating system diversity testing**

![alt text](image-7.png)

---

### **Phase 7: Volume Attachment & Integration**
**Snapshot Data Recovery**
- EBS volume attachment to new instance
- **File system mounting procedures**
- **Cross-instance data accessibility**

![alt text](image-8.png)
![alt text](image-9.png)

---

### **Phase 8: Data Validation & Verification**
**Snapshot Integrity Testing**
```bash
# Expected Output: Hello from task8-instance-1!
```
- **Terminal-based data verification**
- **Successful cross-instance data recovery**

![alt text](image-10.png)

---

## 🚀 **AMI Portability Validation**

### **Phase 9: AMI-Based Instance Launch**
**Template Deployment**
- **One-click instance replication**
- Complete system state restoration
- **Configuration inheritance verification**

![alt text](image-11.png)

---

### **Phase 10: AMI Instance Verification**
**System Integrity Confirmation**
- **Application state preservation**
- **Environment consistency validation**
- **End-to-end replication success**

![alt text](image-12.png)

---

## 📊 **Key Technical Differentiators**

| **Backup Type** | **Scope** | **Use Case** | **Recovery Time** |
|-----------------|-----------|--------------|-------------------|
| **EBS Snapshot** | Block-level storage | Data recovery, volume cloning | Fast (volume-specific) |
| **AMI** | Complete system image | Full instance replication | Moderate (full boot cycle) |

---

## ✅ **Validation Criteria**
- [ ] **Snapshot data accessibility** across different instances
- [ ] **AMI-based instance** functional equivalency  
- [ ] **Cross-platform compatibility** (Ubuntu → RHEL)
- [ ] **Data integrity preservation** throughout backup/restore cycle