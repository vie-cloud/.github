Vielight's Photobiomodulation-Cloud EEG Feedback, Analysis and Translation.

Part of a collaboration with the 2023-2024 McMaster SFWRBME 5P06 Capstone Project Team 28.

# Cloud Architecture
As of April 2024 (Capstone Expo), EEG data is captured, visualized, and processed using a simple algorithm to determine parameters for the Neuro Pro.
![cloud_architecture_diagram_v3-Cloud Architecture - Expo](https://github.com/user-attachments/assets/b6d93469-cb61-4e32-bde7-bb41ad4eac01)

Here is a detailed overview, with dotted lines showing a future state. A future state would include ML models to take in EEG data as training, as well as determine Neuro Pro parameters. Establishing a connection to send the parameters back to the Neuro Pro effectively creates a closed-loop system, as the Neuro Pro parameters will affect EEG signals via photobiomodulation.
![cloud_architecture_diagram_v3-Cloud Architecture](https://github.com/user-attachments/assets/00952502-9818-420b-9b84-28f21c0a481a)

# Data Flow
VieCloud only supports Neuroscan's CURRY for EEG data acquisition. Here is how that data is processed in the VieCloud pipeline to produce Neuro Pro parameters.
<img width="300" alt="image" src="https://github.com/user-attachments/assets/d1ee9647-a435-4182-bdf2-fcb47ebaa034">

# Safety
Authentication is handled by AWS Cognito.
![cloud_architecture_diagram_v3-Login Sequence](https://github.com/user-attachments/assets/a8e50973-8198-4ea9-861e-28b6c472df45)

# UI
## Login Page
<img width="465" alt="image" src="https://github.com/user-attachments/assets/5df2c1a1-04c7-44ab-9fb9-7ce70c6a55cd">

## EEG Dashboard
<img width="641" alt="image" src="https://github.com/user-attachments/assets/25c1cd1c-42d7-41f4-8727-2fd10ecf17ea">

## Parameter Configuration (Automatic)
<img width="418" alt="image" src="https://github.com/user-attachments/assets/cb7c2f96-8c42-4cfd-a5cc-0e17891ae88c">

## Parameter Configuration (Manual)
<img width="303" alt="image" src="https://github.com/user-attachments/assets/65671371-4a08-43f8-a8d9-824b533b8f91">
