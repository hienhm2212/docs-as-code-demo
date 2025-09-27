---
title: "Item"
weight: 2
---

# Item Module
The Item module handles all features about item.

## Key Features
- **Item Management** - Maintain comprehensive medical item database
- **Search Item** - Search item data
## Module Structure

```
{
  "id": "MED-2024-001",
  "name": "Digital Blood Pressure Monitor",
  "description": "Automatic upper arm blood pressure monitor with large LCD display and memory storage for 2 users",
  "category": "Diagnostic Equipment",
  "subcategory": "Cardiovascular Monitoring",
  "manufacturer": "MediTech Solutions",
  "model": "BP-Pro 300",
  "sku": "MT-BP300-001",
  "price": {
    "amount": 89.99,
    "currency": "USD"
  },
  "stock": {
    "quantity": 150,
    "unit": "pieces",
    "warehouse_location": "A-12-03",
    "reorder_level": 25
  },
  "specifications": {
    "dimensions": {
      "length": 12.5,
      "width": 8.2,
      "height": 6.1,
      "unit": "cm"
    },
    "weight": {
      "value": 0.65,
      "unit": "kg"
    },
    "cuff_size": "22-42 cm",
    "memory_capacity": "2 x 99 readings",
    "power_source": "4 AA batteries or AC adapter",
    "display_type": "LCD",
    "accuracy": "±3 mmHg"
  },
  "regulatory": {
    "fda_approved": true,
    "ce_marking": true,
    "iso_certification": "ISO 81060-2:2018",
    "medical_device_class": "Class IIa"
  },
  "availability": {
    "status": "in_stock",
    "shipping_time": "1-3 business days",
    "backorder_allowed": true
  },
  "tags": [
    "blood pressure",
    "cardiovascular",
    "digital",
    "home monitoring",
    "FDA approved",
    "automatic"
  ],
  "created_at": "2024-01-15T10:30:00Z",
  "updated_at": "2024-01-20T14:45:00Z",
  "created_by": "system_admin",
  "supplier": {
    "id": "SUP-001",
    "name": "Global Medical Supplies Inc.",
    "contact": "orders@globalmedsupplies.com"
  },
  "warranty": {
    "duration": 24,
    "unit": "months",
    "coverage": "Manufacturing defects and electronic components"
  }
}
