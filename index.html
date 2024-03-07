<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PSGC API Dropdowns</title>
</head>
<body>
  <label for="region-dropdown">Select Region:</label>
  <select id="region-dropdown">
    <option value="">-- Select Region --</option>
  </select>

  <br>


  <label for="province-dropdown">Select Province:</label>
  <select id="province-dropdown" disabled>
    <option value="">-- Select Province --</option>
  </select>

  <br>

  <label for="city-dropdown">Select City:</label>
  <select id="city-dropdown" disabled>
    <option value="">-- Select City --</option>
  </select>

  <br>

  <label for="barangay-dropdown">Select Barangay:</label>
  <select id="barangay-dropdown" disabled>
    <option value="">-- Select Barangay --</option>
  </select>

  <br>

  <script>
    async function fetchRegionsAndPopulateDropdown() {
      const url = 'https://psgc.gitlab.io/api/regions/';
      
      try {
        const response = await fetch(url);
        const data = await response.json();
        
        const regionDropdown = document.getElementById('region-dropdown');
        data.forEach(region => {
          const option = document.createElement('option');
          option.value = region.code;
          option.textContent = region.name;
          regionDropdown.appendChild(option);
        });
      } catch (error) {
        console.error('Error fetching regions:', error);
      }
    }

    async function fetchProvincesAndPopulateDropdown(regionCode) {
      const url = `https://psgc.gitlab.io/api/regions/${regionCode}/provinces/`; 
      
      try {
        const response = await fetch(url);
        const data = await response.json();
        
        const provinceDropdown = document.getElementById('province-dropdown');
        provinceDropdown.innerHTML = '<option value="">-- Select Province --</option>';
        data.forEach(province => {
          const option = document.createElement('option');
          option.value = province.code;
          option.textContent = province.name;
          provinceDropdown.appendChild(option);
        });
        provinceDropdown.disabled = false;
      } catch (error) {
        console.error('Error fetching provinces:', error);
      }
    }

    async function fetchCitiesAndPopulateDropdown(provinceCode) {
      const url = `https://psgc.gitlab.io/api/provinces/${provinceCode}/cities-municipalities/`; 
      
      try {
        const response = await fetch(url);
        const data = await response.json();
        
        const cityDropdown = document.getElementById('city-dropdown');
        cityDropdown.innerHTML = '<option value="">-- Select City --</option>';
        data.forEach(city => {
          const option = document.createElement('option');
          option.value = city.code;
          option.textContent = city.name;
          cityDropdown.appendChild(option);
        });
        cityDropdown.disabled = false;
      } catch (error) {
        console.error('Error fetching cities:', error);
      }
    }

    async function fetchBarangaysAndPopulateDropdown(cityCode) {
      const url = `https://psgc.gitlab.io/api/cities-municipalities/${cityCode}/barangays/`; 
      
      try {
        const response = await fetch(url);
        const data = await response.json();
        
        const barangayDropdown = document.getElementById('barangay-dropdown');
        barangayDropdown.innerHTML = '<option value="">-- Select Barangay --</option>';
        data.forEach(barangay => {
          const option = document.createElement('option');
          option.value = barangay.code;
          option.textContent = barangay.name;
          barangayDropdown.appendChild(option);
        });
        barangayDropdown.disabled = false;
      } catch (error) {
        console.error('Error fetching barangays:', error);
      }
    }

    document.addEventListener('DOMContentLoaded', fetchRegionsAndPopulateDropdown);

    document.getElementById('region-dropdown').addEventListener('change', function() {
      const regionCode = this.value;
      if (regionCode) {
        fetchProvincesAndPopulateDropdown(regionCode);
      }
    });

    document.getElementById('province-dropdown').addEventListener('change', function() {
      const provinceCode = this.value;
      if (provinceCode) {
        fetchCitiesAndPopulateDropdown(provinceCode);
      }
    });

    document.getElementById('city-dropdown').addEventListener('change', function() {
      const cityCode = this.value;
      if (cityCode) {
        fetchBarangaysAndPopulateDropdown(cityCode); 
      }
    });
  </script>
</body>
</html>
