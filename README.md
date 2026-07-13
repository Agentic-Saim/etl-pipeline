# ETL Pipeline Project

**Author:** [agentic-saim09](https://github.com/agentic-saim09)

This project implements an ETL (Extract, Transform, Load) pipeline that extracts transaction data from an Amazon Redshift data warehouse, performs data cleaning and deduplication, and loads the processed data into an Amazon S3 bucket.

## Project Structure

- `main.py`: The entry point of the pipeline.
- `src/extract.py`: Handles data extraction from Redshift.
- `src/transform.py`: Performs data cleaning and deduplication.
- `src/load_data_to_s3.py`: Handles uploading data to S3.
- `requirements.txt`: Project dependencies.
- `Dockerfile`: Docker configuration for containerized execution.

## Setup and Installation

### Prerequisites

- Python 3.8+
- Docker (optional)

### Environment Variables

Create a `.env` file based on `.env.example` with the following variables:

- `dbname`: Redshift database name
- `host`: Redshift host address
- `port`: Redshift port
- `user`: Redshift username
- `password`: Redshift password
- `aws_access_key_id`: AWS access key ID
- `aws_secret_access_key_id`: AWS secret access key

### Local Execution

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Run the pipeline:
   ```bash
   python main.py
   ```

### Docker Execution

1. Build the image:
   ```bash
   docker build -t etl-pipeline .
   ```

2. Run the container:
   ```bash
   docker run --env-file .env etl-pipeline
   ```

## License

This project is licensed under the Apache2.0 License.

---

---

---

---

---

## Author & Contact

- **Author:** Agentic Saim
- **GitHub:** [@agentic-saim09](https://github.com/agentic-saim09)
- **Email:** [agenticsaim.work@gmail.com](mailto:agenticsaim.work@gmail.com)
- **Profile:** https://github.com/agentic-saim09

