# **FastPipe Automation with UiPath**

**FastPipe Automation** leverages **UiPath** to streamline the bid management process for pipe projects. This automation tool downloads bids, updates the Excel pipeline, sends email notifications, and creates backups—all with minimal manual intervention.

---

## **Features**

- **Automatic Bid Downloading**: Downloads bids from designated states with due dates exactly two weeks from today.
- **Excel Pipeline Update**: Updates the project pipeline in Excel with the latest bids.
- **Automated Email Notifications**: Sends automatic email notifications to relevant parties when new bids are downloaded or updated.
- **FastPipe Integration**: Uploads the downloaded projects directly to **FastPipe** for estimation and further processing.
- **Backup Creation**: Automatically creates backups of downloaded projects in a shared file location.

---

## **Prerequisites**

- **UiPath Studio**: Ensure UiPath Studio is installed on your machine.
- **Microsoft Excel**: For updating the Excel pipeline.
- **SMTP Email Service**: For sending email notifications.
- **FastPipe**: The tool should be set up for integration (if applicable).

---

## **Setup and Configuration**

### **1. Clone the Repository**
   First, clone this repository to your local machine:
   ```bash
   git clone https://github.com/FreddieMwau/Fast_Pipe_Automation.git
   ```

### **2. Import into UiPath Studio**

1. Open UiPath Studio.
2. Go to **Start > Open > Project** and select the folder where you cloned the repository.
3. The project should open with all required workflows.

---

### **3. Configure Variables**

1. Open the `Config.xaml` file.
2. Configure the following variables:
   - **BidSource**: Path to the folder or API where bids are stored.
   - **ExcelPipeline**: Path to your Excel pipeline file.
   - **BackupLocation**: Shared file location for backups.
   - **EmailSettings**: Configure email SMTP settings to send notifications.

---

### **4. Running the Automation**

1. Open `Main.xaml` and run the automation from UiPath Studio.
2. The automation will:
   - Download bids with due dates in the next two weeks.
   - Update the Excel pipeline with new bids.
   - Send email notifications to relevant parties.
   - Upload the projects to **FastPipe**.
   - Create backups of the projects in the designated shared file location.

---

### **5. Schedule Automation (Optional)**

If you want to schedule the automation, you can deploy the project to **UiPath Orchestrator** and schedule it to run at specific times.

---

### **Technologies Used**

- **UiPath**: For automation.
- **Microsoft Excel**: For pipeline updates.
- **SMTP**: For email notifications.
- **FastPipe**: For project estimation.
- **Shared File Storage**: For backups.

## **Contributing**

Contributions are welcome! To contribute:

1. **Fork the Repository**:  
   Click on the "Fork" button in the repository to create a copy in your GitHub account.

2. **Clone the Repository**:  
   Clone your forked repository to your local machine using:
   ```bash
   git clone https://github.com/FreddieMwau/Fast_Pipe_Automation.git
   ```