# **Job portal App**

A modern, feature-rich job management platform built with **React.js**, **Supabase**, **Clerk**, **ShadCN UI**, and **Tailwind CSS**. This application provides an intuitive interface for posting, saving, and managing jobs with seamless authentication and dynamic styling.

---

## **Features**

- **User Authentication**: Powered by Clerk for secure and hassle-free login/signup flows.
- **Job Management**: Post, edit, and delete jobs in real-time with Supabase.
- **Responsive Design**: Built with Tailwind CSS for a stunning UI across all devices.
- **Modular UI Components**: Styled using ShadCN UI for reusable and customizable components.
- **Grid-based Layouts**: Aesthetic and functional grid-based design for managing saved and posted jobs.
- **Developer-Friendly**: Clean code structure and comments for easy understanding and collaboration.

---

## **Technologies Used**

### **Frontend**:
- **React.js**: Core framework for building the application.
- **Tailwind CSS**: For utility-first styling.
- **ShadCN UI**: For modular and customizable component styling.

### **Backend**:
- **Supabase**: Backend-as-a-service for real-time database management and APIs.

### **Authentication**:
- **Clerk**: Handles user authentication and authorization with ease.

---

### **THE SCHEMEA OF PROJECT :

<img width="1119" alt="Screenshot 2024-12-22 at 5 16 06 AM" src="https://github.com/user-attachments/assets/facfe918-12af-4f24-b214-ba4726592ea2" />

### screenshots:
<img width="1415" alt="Screenshot 2024-12-22 at 4 48 43 AM" src="https://github.com/user-attachments/assets/20ee9a78-80e6-4915-aeae-db86e66bf15e" />


<img width="1421" alt="Screenshot 2024-12-22 at 4 49 00 AM" src="https://github.com/user-attachments/assets/b8ee5eb9-8e6f-40f2-b0d3-d71bb5ad42d5" />

<img width="1430" alt="Screenshot 2024-12-22 at 4 49 14 AM" src="https://github.com/user-attachments/assets/df6900e0-6ee3-4aa5-81d6-7e317bd68eb2" />

### The problem i encountered while building this project :

### Error: `PGRST301`

**Details:**
- **Message:** `JWSError JWSInvalidSignature`
- **Code:** `PGRST301`
- **Hint:** N/A


Could not verify JWT: JWSError JWSInvalidSignature ??????
it took my hour to figure to it tho
but it was easy
TWO WAYS TO SOLVE IT !!!!!
Way First:
1. **Install the Supabase CLI**  
   If you haven't already installed the Supabase CLI, follow the [installation guide](https://supabase.com/docs/guides/cli) for your operating system.

2. **Start Supabase Locally**  
   Run the following command to start the local Supabase instance:
   ```bash
   supabase start
3.**Get the New Anon Key
After running supabase start, you will see the SUPABASE_ANON_KEY in the output. Copy this key.

Update the .env File
Replace the old SUPABASE_ANON_KEY in your project's .env file with the new key you obtained in the previous step


### WAY SECOND:

i went to clerk dashboard firstly and changed my jwt secret key which i got from supabase api section and update it and DAMMMMM it WORKED FOR ME !!!!! after so many hours anyways ,
HAPPY CODING !!!!!!!!







## **Installation**

Follow these steps to get the project up and running locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/job-manager-app.git
   cd job-manager-app
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

3. **Set Up Environment Variables**:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     VITE_SUPABASE_URL=your_supabase_url
     VITE_SUPABASE_KEY=your_supabase_key
     VITE_CLERK_FRONTEND_API=your_clerk_frontend_api
     ```

4. **Run the Application**:
   ```bash
   npm run dev
   ```

5. **Access the App**:
   Open [http://localhost:5173](http://localhost:5173) in your browser.

---


