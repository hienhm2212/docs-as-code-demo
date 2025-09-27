---
title: "Submit Pre-requisition"
weight: 1
description: "Learn how to submit pre-requisition requests in the MIMS system"
icon: "send"
date: "2025-01-27T10:00:00+07:00"
lastmod: "2025-01-27T10:00:00+07:00"
draft: false
toc: true
author: "Hien Huynh-Minh"
version: "0.1"
---

# Submit Pre-requisition

The Submit Pre-requisition feature allows authorized users to create and submit pre-requisition requests for medical items, equipment, or services within the MIMS system.

## Overview

Pre-requisition submission is a critical workflow in the medical inventory management process. It enables departments to request items before they are needed, ensuring proper planning and resource allocation.

## Prerequisites

Before submitting a pre-requisition, ensure you have:

- **Valid User Account** - Active MIMS user account with appropriate permissions
- **Department Access** - Access to the department for which you're submitting the request
- **Item Information** - Complete details about the items you need to request
- **Budget Approval** - Confirmed budget allocation for the requested items

## Step-by-Step Guide

### Access the Submit Form

1. Navigate to **Modules** → **Pre-requisition** → **Submit**
2. Click the **"New Pre-requisition"** button
3. The submission form will open in a new window

### Fill Basic Information

Complete the following required fields:

| Field | Description | Example |
|-------|-------------|---------|
| **Request ID** | Auto-generated unique identifier | PR-2025-001234 |
| **Department** | Your department name | Surgery Department |
| **Requested By** | Your full name | Dr. John Smith |
| **Request Date** | Current date (auto-filled) | 2025-01-27 |
| **Priority Level** | Urgency of the request | High, Medium, Low |
| **Expected Delivery** | When items are needed | 2025-02-15 |

### Add Items to Request

#### Adding Individual Items

1. Click **"Add Item"** button
2. Search for the item using:
   - Item code
   - Item name
   - Category
3. Enter the required quantity
4. Add any special notes or specifications
5. Click **"Add to Request"**

#### Bulk Item Import

For multiple items, you can:

1. Download the **Item Template** (Excel format)
2. Fill in the template with item codes and quantities
3. Upload the completed template
4. Review imported items before submission

### Item Details Example

```yaml
Item Request Example:
  - Item Code: MED-001
  - Item Name: Surgical Gloves (Sterile)
  - Category: Personal Protective Equipment
  - Quantity: 500 boxes
  - Unit: Boxes
  - Specifications: Latex-free, Size M
  - Estimated Cost: $2,500.00
  - Notes: Required for upcoming surgical procedures
```

### Review and Submit

1. **Review Summary** - Check all entered information
2. **Validate Budget** - Ensure sufficient budget allocation
3. **Attach Documents** - Upload any supporting documents (optional)
4. **Add Comments** - Include any additional notes
5. **Submit Request** - Click **"Submit Pre-requisition"**

## Form Validation

The system performs several validation checks:

- **Required Fields** - All mandatory fields must be completed
- **Item Availability** - Items must exist in the system catalog
- **Quantity Limits** - Quantities must be within acceptable ranges
- **Budget Validation** - Total cost must not exceed department budget
- **Date Validation** - Expected delivery date must be in the future

## Status Tracking

After submission, you can track your pre-requisition status:

| Status | Description |
|--------|-------------|
| **Submitted** | Request received and `under` review |
| **Under Review** | Being evaluated by department head |
| **Approved** | Approved and forwarded to procurement |
| **Rejected** | Rejected with reason provided |
| **In Progress** | Items being sourced and ordered |
| **Completed** | Items delivered and request fulfilled |

## Common Use Cases

### Emergency Requests

For urgent medical supplies:

1. Select **"High Priority"** level
2. Add **"Emergency"** tag to the request
3. Include detailed justification in comments
4. Contact department head for immediate approval

### Seasonal Stocking

For regular inventory replenishment:

1. Use **"Medium Priority"** level
2. Plan ahead for seasonal demand
3. Include historical usage data
4. Coordinate with other departments

### New Equipment Requests

For capital equipment purchases:

1. Attach detailed specifications
2. Include vendor quotes (if available)
3. Provide justification for purchase
4. Ensure proper approval workflow

## Best Practices

### Before Submission

- **Plan Ahead** - Submit requests well in advance of need
- **Accurate Quantities** - Use historical data to estimate quantities
- **Clear Specifications** - Provide detailed item specifications
- **Budget Planning** - Ensure adequate budget allocation

### During Submission

- **Double-Check Information** - Verify all entered data
- **Complete Documentation** - Include all required attachments
- **Clear Communication** - Use descriptive comments and notes

### After Submission

- **Monitor Status** - Regularly check request status
- **Respond to Queries** - Promptly answer any clarification requests
- **Update Information** - Modify requests if requirements change

## Troubleshooting

### Common Issues

- **Issue**: "Item not found in catalog"
  **Solution**: Verify item code or contact inventory manager

- **Issue**: "Budget exceeded"
  **Solution**: Reduce quantities or request budget increase

- **Issue**: "Invalid delivery date"
  **Solution**: Ensure date is in the future and realistic

- **Issue**: "Submission failed"
  **Solution**: Check internet connection and try again

### Getting Help

If you encounter issues:

1. Check the **Help Documentation**
2. Contact your **Department Administrator**
3. Submit a **Support Ticket**
4. Call **IT Helpdesk**: +1-555-0123

## Related Documentation

- [Pre-requisition Overview](../_index.md)
- [Item Management](../../item/index.md)
- [User Management](../../user/index.md)
- [Approval Workflow](../../approval/index.md)

## API Reference

For developers integrating with the pre-requisition system:

```javascript
// Submit pre-requisition via API
POST /api/v1/prerequisites
{
  "department": "Surgery Department",
  "requestedBy": "Dr. John Smith",
  "priority": "High",
  "expectedDelivery": "2025-02-15",
  "items": [
    {
      "itemCode": "MED-001",
      "quantity": 500,
      "notes": "Required for upcoming procedures"
    }
  ],
  "comments": "Emergency surgical supplies needed"
}
```

## Code Examples

### Ruby
```ruby
class User
  def initialize(name)
    @name = name
  end

  def greet
    puts "Hello, #{@name}!"
  end
end

user = User.new("Alice")
user.greet
```

### Go
```go
package main

import "fmt"

func main() {
    name := "World"
    fmt.Printf("Hello, %s!\n", name)
}
```

### React.js
```jsx
import React from 'react';

const Greeting = ({ name }) => {
  return <h1>Hello, {name}!</h1>;
};

export default Greeting;
```
