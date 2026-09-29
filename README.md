F/ND/25/3210143
Idowu basit Mayowa 

# 1.Feature: Automated SKU Generation & Variant Identification

## Short Description
A system that automatically creates unique, structured Stock Keeping Unit (SKU) codes for every product and its variants (size, colour, style, etc.) based on predefined business rules, while also supporting manual override and bulk generation for existing items.

## Purpose
To eliminate duplicate or inconsistent product identifiers, reduce human error during item creation, and provide a reliable, machine-readable way to uniquely identify every stockable item across the inventory system. This forms the foundation of accurate item identification and enables all downstream store-keeping activities.

## Main Functions / Activities
- Define and store SKU naming templates/rules (e.g., Category-Brand-Attribute-Sequence)
- Auto-generate unique SKUs when a new item or variant is created
- Bulk-generate missing SKUs for existing catalogue items
- Support multiple identifiers per item (primary SKU + UPC/EAN/barcode + vendor part number)
- Validate uniqueness of every generated SKU before saving
- Allow controlled manual editing of SKUs with audit logging
- Link parent products to their variant SKUs for hierarchical identification
- Export/import SKU master data for synchronisation with other systems


# 2.Feature: Real-Time Stock Level Tracking with Reorder Points

## Short Description
Core store-keeping functionality that continuously tracks the quantity of every SKU on hand, available, committed, and on order, and automatically triggers low-stock alerts or purchase recommendations when stock falls to a defined reorder point.

## Purpose
To maintain accurate physical stock visibility at all times and prevent stockouts or overstocking. This is a fundamental store-keeping capability that ensures the business always knows what is available, what needs replenishment, and when to reorder—directly supporting efficient day-to-day inventory control.

## Main Functions / Activities
- Maintain live quantities per SKU: On Hand, Available, Committed/Allocated, On Order
- Set and manage reorder points (minimum level) and preferred replenishment levels (maximum/target) per SKU
- Automatically generate low-stock alerts or notifications when quantity reaches the reorder point
- Support manual stock adjustments with reason codes and full history
- Record all stock movements (receipts, sales, transfers, adjustments) against the correct SKU
- Provide quick views of current stock status filtered by category, location, or low-stock status
- Allow bulk update of reorder points across multiple SKUs
- Keep an auditable movement history for every quantity change
