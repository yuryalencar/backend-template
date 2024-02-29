Scripts de automação: Mantenha scripts úteis para tarefas de automação, como migrações de banco de dados ou inicialização do servidor.

Example of the code for scripts/migrateDatabase.ts:
```
import databaseMigrator from '../database/migrate';

async function migrateDatabase() {
  // Implement logic to migrate the database
  await databaseMigrator.runMigrations();
  console.log('Database migrated successfully');
}

migrateDatabase();
```
