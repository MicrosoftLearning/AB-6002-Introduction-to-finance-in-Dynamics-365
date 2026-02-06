## Demo: Global address book

This demo shows how the global address book works and explains the type of data you can store in the address book versus directly in the legal entity records.

### Setup

No custom setup required. Will use the System administrator Admin account and will create the 2 customers right within the demo.

## Script

In this demo, we explore the global address book, which is a central storage location for people and organizations known to our finance and operations apps environment. The people and organizations are called parties. Examples include employees, customer accounts, vendor accounts, and contacts for customers and vendors. The global address book stores name and address information and is shared across the legal entities defined. Most other information for people and organizations is stored directly in the legal entity.

Let’s start by creating a new customer account in legal entity USMF. I’ll name this account Coho Winery. The URL is cohowinery.com. The phone number for Coho Winery is 707-555-0106. Next, we’ll enter the address:

303 Vineyard Road

Napa, CA 90001 USA

Now we’ll switch to our German legal entity, DEMF.

Contoso, Ltd. Germany has the same customer, Coho Winery. We want the customer in DEMF linked to the customer in USMF and the address and other contact information should stay in sync as we make changes. As we create the new customer in DEMF, the system recognizes that a customer with this name already exists and asks if we want to use that customer. When we respond yes, these records become linked to the same party in the global address book. Since the party holds addresses and contact information, what we entered in USMF is displayed for our DEMF customer.

The customer has a change in address. We can make this change in either the USMF or DEMF legal entity. Since we are in DEMF right now, let’s change it here. The new address is 304 Vineyard Road (just a small change).

Now switch back to legal entity USMF and find this same customer. Notice how the address has changed here.

What about payment terms? I’ll change **payment terms** to **Net10** in the **Payment defaults** FastTab in my USMF customer. Now change to the DEMF customer. It doesn’t change there. Payment terms are not part of the address information and are not stored in the global address book.

Let’s navigate to the global address book. It’s available in a couple of places, but I’ll navigate to **Common \> Common \> Global address book**. Enter **C**oho Winery in the quick filter to find our customer. Expand the **Address** FastTab and notice that the new address is stored here. The party number that is shared for the customers in each of the 2 legal entities is displayed here.

Coho Winery also manufactures certain compounds that we need in our US manufacturing company (USMF). We need to define them as a vendor as well and track that they are the same company. Navigate to **Accounts payable \> Vendors \> All vendors**. Select **New** to create a new vendor. When you start typing the name, the application lets you know we already have that entry in the global address book and you are able to select it. This will link the new vendor to the same party.

Back to the **global address book**—let’s review the party. Open the **Roles** FastTab. Notice that this party is linked to a customer in USMF, a customer in DEMF, and a vendor in USMF.


