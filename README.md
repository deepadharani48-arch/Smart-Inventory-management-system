# SMART INVENTORY MANAGEMENT SYSTEM
> **"Smarter Stock Control. Better Business Decisions."**  
> *Academic Final-Year Project • Enterprise Frontend Web Application*

A modern, responsive, commercial-grade Frontend-Only Inventory Management SaaS platform designed for warehouse operations, logistics monitoring, stock auditing, and executive business analytics.

Built entirely with **React 19**, **Vite**, **Tailwind CSS v4**, **Recharts**, and **Lucide React**, powered by persistent browser **LocalStorage**.

---

## 🌟 Key Features & Capabilities

### 1. Operations Dashboard
- **6 Real-time Stat Cards** calculated dynamically from active data:
  - Total Products in catalog
  - Total Stock Units in warehouse
  - Low Stock Warning items
  - Critical Out-of-Stock items
  - Total Inventory Valuation (Selling Price & Cost Investment)
  - Departmental Categories
- **Monthly Inventory Activity Trend** (Recharts AreaChart: Inbound vs Outbound shipments).
- **Stock Share Distribution** (Recharts PieChart by product category).
- **Top Stock Holdings** (Ranked by volume or total valuation).
- **Low-Stock Alert Center** with 1-click **"Restock"** action buttons.
- **Recent Stock Movements** audit feed with live status badges.

### 2. Comprehensive Product Management
- Catalog table and modern visual card grid views.
- High-resolution product images and category color badges.
- **Add Product Modal** with real-time field validation (positive pricing, min threshold, SKU formatting).
- **Edit Product Modal** with instant state synchronization.
- **Delete Product** with safety confirmation dialog.
- **Multi-criteria Filtering & Sorting**:
  - Live global search (Name, SKU, Category, Supplier, Location)
  - Filter by Category dropdown
  - Filter by Stock Status (Healthy, Low Stock, Out of Stock)
  - Column sorting (Name, Price, Stock Units, Date Modified)
  - Pagination controls with configurable page sizes (5, 10, 20 items per page).

### 3. Strict Stock Transaction Management
- **Stock In (PO)**: Receive stock from suppliers, purchase orders, or customer returns.
- **Stock Out (SO)**: Dispatch stock for sales or inter-department transfers.
  - *Strict Validation*: Prevents stock quantities from falling below zero; triggers clear warning toasts if requested quantity exceeds current availability.
- **Stock Adjustment**: Reconcile physical warehouse audits, damaged units, or inventory shrinkage.
- **Complete Movement Audit Trail**: Records transaction timestamp, reference order number, quantity change, before/after balances, operator name, and notes.

### 4. Category & Supplier Management
- Dedicated **Categories Page**: Add, edit, and delete categories with custom color pickers and live valuation totals.
- Dedicated **Suppliers Directory**: Track vendor contact information, lead times, reliability ratings, and link directly to supplied products.

### 5. Reports & Financial Intelligence
- Financial valuation breakdown: Total Retail Value, Total Cost, Projected Gross Margin, and Average Unit Value.
- Departmental inventory valuation comparison chart (Recharts BarChart).
- **3 Real-time CSV Data Exports**:
  1. *Products Master Catalog CSV*
  2. *Stock Movement & Audit Trail CSV*
  3. *Critical Low-Stock Reorder Report CSV*

### 6. Automated Alerts & Notification Center
- Instant triggers when stock reaches zero or falls below minimum thresholds.
- Notification badges with unread counters in the top navigation bar.
- Dedicated Alerts Center with priority filtering (Critical, Warning, Replenishment).
- Direct "Restock Now" shortcut buttons within alert items.

### 7. Customization & System Settings
- Enterprise branding configuration (Store/Company name, Warehouse ID, contact email).
- **Multi-Currency Support**: Switch between `$ USD`, `€ EUR`, `£ GBP`, `₹ INR`, `¥ JPY`, `A$ AUD`, and `C$ CAD`.
- **Theme Selection**: Seamless Light Mode and Dark Mode switching.
- **Full JSON Database Backup & Restore**: Export and import complete database snapshots.
- **Reset to Demo Data**: One-click restore back to the original demo dataset at any time.

---

## 🛠️ Technology Stack

- **Framework**: React 19 (Hooks, Context API)
- **Bundler & Dev Server**: Vite 8
- **Styling**: Tailwind CSS v4 & Modern Glassmorphism
- **Charts & Data Visualizations**: Recharts
- **Icons**: Lucide React
- **Data Persistence**: Browser LocalStorage (Zero backend or API dependencies required)

---

## 🚀 Getting Started

### 1. Navigate to the project directory
```bash
cd "C:\Users\nagar\.gemini\antigravity\scratch\smart-inventory-system"
```

### 2. Start the local development server
```bash
npm run dev
```

### 3. Open in your browser
Visit:
```
http://localhost:5173
```

---

## 🎓 Project Demonstration & Presentation Tips

1. **Dashboard Demonstration**:
   - Point out that all numbers on the top cards are dynamically calculated from the browser's database.
   - Highlight the interactive Recharts graphs with custom tooltips.

2. **Stock In / Out Demonstration**:
   - Open **Stock Management** -> Click **Stock Out**.
   - Select an item (e.g., Logitech MX Master 3S) and try to dispatch more than available stock to showcase the negative stock prevention logic.
   - Dispatch an acceptable quantity and show how the product quantity, status badge, and dashboard cards update instantly.

3. **Restock from Alert**:
   - Show how a low-stock alert provides a 1-click **"Restock"** action that pre-selects the product and handles the inbound receipt.

4. **CSV Exporting**:
   - Go to **Reports & Analytics** and click **Export Products CSV** or **Movements CSV** to show that a real, structured `.csv` file is downloaded.

5. **Demo Reset**:
   - Mention that judges or recruiters can experiment freely with creating/deleting items and then click **"Reset Demo Data"** in Settings or user menu to restore the original catalog.

---

*Smart Inventory Management System | Academic Project*
