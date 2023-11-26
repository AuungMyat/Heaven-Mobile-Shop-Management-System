# Heaven-Mobile-Shop-Management-System
For the admin account:
Username: Admin
Password: Admin

For the Cashier account:
Username: Cashier
Password: Cashier

For the database, You need to create your own MS MySQL Database. I will provide with the SQL Query Scripts:

The Database Name is: HeavenDB

For the Table,
Table name: MobileTbl
CREATE TABLE [dbo].[MobileTbl] (
    [MobileID] INT          NOT NULL,
    [MBrand]   VARCHAR (30) NOT NULL,
    [MModel]   VARCHAR (30) NOT NULL,
    [MPrice]   INT          NOT NULL,
    [MStock]   INT          NOT NULL,
    [MRam]     INT          NOT NULL,
    [MRom]     INT          NOT NULL,
    [MCam]     INT          NOT NULL,
    PRIMARY KEY CLUSTERED ([MobileID] ASC)
);

Table name: AccessoriesTbl
CREATE TABLE [dbo].[AccessoriesTbl] (
    [AccessoriesID] INT          NOT NULL,
    [ABrand]        VARCHAR (20) NOT NULL,
    [AModel]        VARCHAR (20) NOT NULL,
    [AStock]        INT          NOT NULL,
    [APrice]        INT          NOT NULL,
    PRIMARY KEY CLUSTERED ([AccessoriesID] ASC)
);

Table name: BillTbl
CREATE TABLE [dbo].[BillTbl] (
    [Billid]     INT          NOT NULL,
    [ClientName] VARCHAR (50) NULL,
    [Amt]        INT          NULL,
    PRIMARY KEY CLUSTERED ([Billid] ASC)
);

