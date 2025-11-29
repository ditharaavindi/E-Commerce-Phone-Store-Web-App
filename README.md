# Y02S2_Project-Ecommerce-Mobileshop

A responsive web app for an online store selling phones and tech accessories.
Allows customers to browse and order mobile accessories online. The shop owner can manage products, view orders
Features include user authentication, admin dashboard, product search, shopping cart with checkout, customer reviews, and support center, wishlist

**Prerequisites:**

- **Node.js** (recommended v18+)
- **npm** (comes with Node) or **yarn**
- **Java 17** (required by the Spring Boot backend)
- **MySQL** (local or remote database)
- **Maven** (optional if you use the included `mvnw` wrapper)

**Quick Start — Backend (Spring Boot)**

- Change to the backend directory:

  `cd Backend/MackTech/MackTech`

- (Optional) Build the project:

  `./mvnw clean package`

- Run the application (uses the included Maven wrapper):

  `./mvnw spring-boot:run`

- Or run the built jar after packaging:

  `java -jar target/MackTech-0.0.1-SNAPSHOT.jar`

Notes:

- The backend expects a MySQL database. The default connection is configured in `src/main/resources/application.properties`. Update the `spring.datasource.username` and `spring.datasource.password` values as needed.
- Example: import the provided SQL schema/data (from the repository root) with:

  `mysql -u root -p < ./SQL-Dummy.sql`

**Quick Start — Frontend (React + Vite)**

- Change to the frontend directory:

  `cd Frontend`

- Install dependencies:

  `npm install`

- Run the dev server (with hot reload):

  `npm run dev`

- Build for production:

  `npm run build`

- Preview a production build locally:

  `npm run preview`

**Ports & defaults**

- Backend default port: `8080` (configurable in `application.properties`)
- Frontend dev server default port: `5173` (Vite default)

**Troubleshooting**

- If the backend cannot connect to MySQL, verify that MySQL is running and the credentials/database name in `application.properties` are correct.
- If ports are already in use, change them (`server.port` for Spring Boot; pass `--port` to Vite or set `PORT` env var for the frontend).
- If you don't have Maven installed, use the included wrapper `./mvnw` (Unix/macOS) as shown above.

If you'd like, I can also add a short `Makefile` or shell script to simplify these commands.
