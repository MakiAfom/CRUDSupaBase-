# CRUDSupa-Base-Prisma
Prisma & Supabase Tutorial
#Prerequisites
•	Docker is installed and running
Setup
•	Install dependencies: npm install

Start Supabase: 
•	npx supabase start or npm run db-start
Migrate & Seed:
•	npm run init

Migrations
Applying Migrations: 
•	npx prisma migrate deploy
Creating a new migration file: 
•	npx prisma migrate dev --name [NAME]
Pushing schema to database without migration: 
•	npx prisma db push

Code Generation
Create Prisma client & types without migrating:
•	npx prisma generate

Generate Supabase types from Database: 
•	npx supabase 
•	gen types typescript --local --schema 
•	public > src/types/supabaseTypes.ts or
•	 npm run update-types

Seeding & Querying
Running Seed: 

•	npx prisma db seed
Querying via SupaBase client (data API): 
•	npx ts-node src/supabase.ts
Querying via Prisma client: 
•	npx ts-node src/prisma.ts


